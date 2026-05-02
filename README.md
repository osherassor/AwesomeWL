# AwesomeWL

> Curated wordlists for web application content discovery and subdomain enumeration — built for the modern stack (2025–2026).

`AwesomeWL` is a pair of high-signal wordlists for bug bounty hunters, pentesters, and red teamers who are tired of stale 2018-era lists that miss everything modern developers actually deploy: AI assistant configs, MCP servers, edge runtimes, vector DBs, agent frameworks, and the long tail of `.md` files engineers commit by accident.

---

## What's inside

| File | Lines | Purpose |
|---|---:|---|
| [`Common_list.txt`](Common_list.txt) | **25,265** | Files & directories for content discovery (`ffuf`, `feroxbuster`, `gobuster`, `dirsearch`) |
| [`subdomains`](subdomains) | **5,146** | Subdomain candidates for DNS brute-forcing (`puredns`, `shuffledns`, `amass`) |

### `Common_list.txt` — what makes it different

Most wordlists were last seriously updated when jQuery was still in fashion. This one tracks what's actually deployed in 2025–2026:

- **AI coding assistants** — `CLAUDE.md`, `AGENTS.md`, `.cursor/`, `.cursorrules`, `.windsurfrules`, `.aider.*`, `.cline*`, `.roo*`, `.codex`, `.continue/`, `.codeium/`, `.zed/`, `.github/copilot-instructions.md`
- **Model Context Protocol (MCP)** — `.mcp.json`, `claude_desktop_config.json`, `smithery.yaml`
- **AI app builders** — Lovable, Base44, Wix/Velo, Bolt.new, v0.dev, Replit
- **Open agent platforms** — OpenCode, OpenHands, LibreChat, Goose, Ollama, Jan, Msty, AnythingLLM, Open WebUI
- **Agent frameworks** — LangGraph, LangChain, LlamaIndex, Mastra, Inngest, Trigger.dev, CrewAI, AutoGen, Letta, n8n, Flowise, Dify
- **ML ops & inference** — Modal, Replicate, RunPod, BentoML, MLflow, Weights & Biases, Comet
- **Vector databases** — Pinecone, Weaviate, Qdrant, Chroma, Milvus, LanceDB, Vespa, Turbopuffer
- **2025 web frameworks** — TanStack Start, Solid, Qwik, Hono, Elysia, Wasp, Encore, Effect, EdgeDB, Astro, Fresh, RedwoodJS
- **Modern build tools** — Bun, Deno, Biome, Turbo, Nx, Rolldown, Oxc, Farm, Lightning CSS
- **Edge / serverless** — Cloudflare Wrangler, Fly.io, Railway, SST v3, Pulumi, OpenTofu, AWS CDK, Amplify Gen 2
- **Auth (2025)** — Clerk, WorkOS, Stytch, Kinde, Logto, Authelia, Authentik, Supertokens, Better-Auth, Auth.js, Lucia
- **Modern data layer** — Turso, Neon, PlanetScale, Xata, libSQL, ElectricSQL, Triplit, InstantDB, Powersync, Drizzle, Convex, Supabase, Pglite
- **Realtime / sync** — Liveblocks, PartyKit, Replicache, Automerge, Yjs
- **Modern Python** — `uv.lock`, `ruff.toml`, `pyrightconfig.json`, Marimo, Dagster, Prefect, Polars, DuckDB
- **Native / mobile** — Tauri, Capacitor, Expo (`eas.json`), Swift Package, KMP, fastlane
- **K8s / containers** — Helm, Kustomize, Tilt, Skaffold, Earthly, Dagger, Flux, Argo, Podman
- **Observability** — OpenTelemetry, Sentry, Datadog, Honeycomb, Axiom, Highlight, PostHog, Tinybird
- **Security tooling configs** — Trivy, Snyk, Semgrep, Gitleaks, Trufflehog, Aikido
- **Secret managers** — Doppler, Infisical, Vault, sops, age
- **Headless CMS** — Sanity, Payload, Strapi, Tina, Hygraph, Contentlayer, KeyStatic, Velite
- **Modern testing** — Vitest, Playwright, Cypress, Storybook 8, Knip, Stryker
- **macOS dev artifacts** — `.fseventsd`, `.Spotlight-V100`, `.TemporaryItems`, `Info.plist`, `xcuserdata`, `Pods`, `.swiftpm`, `.icloud`
- **Internal `.md` docs** (high signal for OSINT) — `TODO.md`, `NOTES.md`, `ROADMAP.md`, `ARCHITECTURE.md`, `RUNBOOK.md`, `SECRETS.md`, `THREAT_MODEL.md`, `POSTMORTEM.md`, `INTERNAL.md`
- **~935 paths from latest [nuclei-templates](https://github.com/projectdiscovery/nuclei-templates)** — `http/exposures`, `exposed-panels`, `misconfiguration`, `files`, `vulnerabilities`

Plus the full classic SecLists / RAFT / dirbuster heritage carried forward.

---

## Why these specific entries?

Each new entry was chosen because it has a meaningful chance of leaking one of:

1. **Secrets** — API keys, OAuth tokens, DB credentials (`.env.production.local`, `firebase-adminsdk.json`, `wrangler.toml`)
2. **Prompts & system instructions** — agent rules, system prompts (`CLAUDE.md`, `.cursorrules`, `system-prompt.md`)
3. **Architecture & internals** — internal docs, threat models, runbooks (`ARCHITECTURE.md`, `THREAT_MODEL.md`, `INTERNAL.md`)
4. **Infrastructure config** — Terraform state, Pulumi configs, k8s manifests (`terraform.tfstate`, `Pulumi.production.yaml`)
5. **Source maps & generated code** — type definitions, generated GraphQL schemas, `payload-types.ts`

No wildcards, no regex — every entry is a literal path, fuzz-ready as-is.

---

## Usage

### Content discovery with `ffuf`

```bash
ffuf -w Common_list.txt -u https://target.com/FUZZ -mc 200,204,301,302,307,401,403 -fs 0
```

### Recursive discovery with `feroxbuster`

```bash
feroxbuster -u https://target.com -w Common_list.txt -x php,html,json,yaml,md,env -d 3
```

### Discovery with `gobuster`

```bash
gobuster dir -u https://target.com -w Common_list.txt -x php,json,yaml -t 50
```

### Subdomain brute-force with `puredns`

```bash
puredns bruteforce subdomains target.com -r resolvers.txt -w resolved.txt
```

### Subdomain brute-force with `shuffledns`

```bash
shuffledns -d target.com -w subdomains -r resolvers.txt -mode bruteforce
```

---

## Notes on case-sensitivity

The list intentionally contains both case variants for high-value files (`AGENTS.md` and `agents.md`, `CLAUDE.md` and `claude.md`). Linux web servers are case-sensitive — fuzzing only one case misses the other.

---

## Contributing

Pull requests welcome. New entries should:

- Be a **literal file or folder name**, not a wildcard or pattern
- Correspond to a real, currently-shipping tool or framework
- Have plausible leak value (config, secrets, prompts, internals, generated code)
- Be checked against the existing list to avoid exact duplicates

Open a PR with a brief note on what tool/framework the entries target and roughly when it became popular.

---

## Credits

Built and maintained by [@osherassor](https://github.com/osherassor).

Heritage: classic dirbuster / RAFT / SecLists, extended with modern tooling that those lists predate.
