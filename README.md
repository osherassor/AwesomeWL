<h1 align="center">AwesomeWL</h1>

<p align="center">
  <strong>High-signal wordlists for modern web recon, internal pentesting, and bug bounty.</strong><br>
  Built for the 2025–2026 stack — AI assistants, MCP servers, edge runtimes, vector DBs, agent frameworks, and the long tail of files engineers commit by accident.
</p>

<p align="center">
  <img src="https://img.shields.io/github/stars/osherassor/AwesomeWL?style=for-the-badge&logo=github&color=ffd700" alt="Stars">
  <img src="https://img.shields.io/github/last-commit/osherassor/AwesomeWL?style=for-the-badge&logo=git&color=00d4aa" alt="Last commit">
  <img src="https://img.shields.io/badge/entries-35%2C330-blueviolet?style=for-the-badge" alt="Total entries">
  <img src="https://img.shields.io/badge/license-MIT-informational?style=for-the-badge" alt="License">
</p>

---

## What's inside

| File | Lines | Purpose |
|---|---:|---|
| [`Common_list.txt`](Common_list.txt) | **25,265** | Files & directories — content discovery (`ffuf`, `feroxbuster`, `gobuster`, `dirsearch`, `katana`) |
| [`subdomains`](subdomains) | **10,065** | Subdomain candidates — internal + external recon (`puredns`, `shuffledns`, `amass`, `LANWhisper`) |
| [`subdomains_quick_win.txt`](subdomains_quick_win.txt) | **100** | Top-100 lateral-movement targets for internal pentest — fastest path to creds, code execution, or DA |

Most public wordlists were last seriously refreshed when jQuery was still in fashion. AwesomeWL extends the classic SecLists / dirsearch / dirbuster heritage with **~5,000 modern entries** that target what teams actually deploy today: Claude / Cursor / Aider configs, MCP servers, Wrangler `.dev.vars`, Drizzle / Convex schemas, AI agent prompt files, and Cloudflare Workers internals.

---

## Tools that use AwesomeWL

### 🔉 [LANWhisper](https://github.com/osherassor/LANWhisper) — Internal DNS recon

LANWhisper is the **companion tool** for `subdomains` — a Python CLI that resolves a list of asset hostnames against system or custom DNS servers and produces JSON / CSV / HTML / TXT reports. It pairs naturally with `AwesomeWL/subdomains` because the list was deliberately built for **both internal and external recon** (corporate AD trees, OOB management, M365/Skype federation, plus modern SaaS / AI / edge platforms).

```bash
# Install LANWhisper
git clone https://github.com/osherassor/LANWhisper && cd LANWhisper
python3 -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt

# Pull the AwesomeWL subdomain list
curl -sO https://raw.githubusercontent.com/osherassor/AwesomeWL/main/subdomains

# Internal sweep against a corporate DNS server, stealth mode
./lanwhisper.py \
    --domain corp.local \
    --server 10.0.0.53 \
    --source ./subdomains \
    --stealth \
    --output ./out

# External sweep against an in-scope target
./lanwhisper.py \
    --domain target.com \
    --source ./subdomains \
    --workers 128 \
    --output ./out
```

Outputs go to `./out/run_YYYYMMDD_HHMMSS_<id>/` — JSON for piping, CSV for spreadsheets, HTML for client reports, TXT for the terminal.

> **Why this combo:** the wordlist is balanced for hybrid environments. It hits classic AD targets (`vcenter`, `idrac`, `cyberark`, `wazuh`), modern SaaS (`clerk`, `supabase`, `posthog`), AI products (`mcp-gateway`, `prompt-firewall`, `agent-router`), and the environment / region / cluster matrix (`qa1..3`, `eu-west-1-internal`, `node-01..10`) that real corp networks actually use.

---

## Usage with other tools

### Content discovery

```bash
# ffuf — fast, with status filtering
ffuf -w Common_list.txt -u https://target.com/FUZZ \
     -mc 200,204,301,302,307,401,403 -fs 0 -t 50

# feroxbuster — recursive, with extensions
feroxbuster -u https://target.com -w Common_list.txt \
     -x php,html,json,yaml,md,env,bak -d 3

# gobuster
gobuster dir -u https://target.com -w Common_list.txt \
     -x php,json,yaml,bak -t 50

# katana — for crawling-augmented discovery
katana -u https://target.com -d 3 -jc -w Common_list.txt

# nuclei (fuzzing-templates with custom wordlist)
nuclei -u https://target.com -t fuzzing-templates/ -V wordlist=Common_list.txt
```

### Subdomain brute-force

```bash
# puredns — fastest pure brute-force
puredns bruteforce subdomains target.com \
     -r resolvers.txt -w resolved.txt

# shuffledns
shuffledns -d target.com -w subdomains \
     -r resolvers.txt -mode bruteforce

# amass — pair with subdomains as alteration source
amass enum -d target.com -brute -w subdomains \
     -src -o amass.out

# dnsx — resolve and validate
sed "s/$/.target.com/" subdomains | dnsx -resp -silent

# alterx — generate permutations from your already-found subs
echo target.com | alterx -en "subdomains" | dnsx -silent
```

### Internal pentest workflow

```bash
# 1. Resolve internal-flavored entries against the corp DNS
./lanwhisper.py --domain corp.local --server 10.0.0.53 \
                --source subdomains --stealth -o ./scope

# 2. Filter for live HTTP services
cat scope/run_*/results.csv | cut -d, -f3 | sort -u \
    | httpx -title -tech-detect -status-code -o live.txt

# 3. Hit the live ones with the file wordlist
xargs -I {} -a live.txt ffuf -w Common_list.txt -u {}/FUZZ -mc 200,401,403
```

---

## What makes the lists different

### `subdomains_quick_win.txt` — 100 lateral-movement targets

A focused 100-entry list for **internal pentest first-blood**. Run it first against the corp DNS — every hit is a system that, when compromised, typically yields one of: source code + pipeline secrets, plaintext domain credentials, code-push to other hosts, or full hypervisor / backup access.

```bash
./lanwhisper.py --domain corp.local --server 10.0.0.53 \
                --source subdomains_quick_win.txt --output ./quick_win
```

**Categories** (rough tier-1 lateral-movement value):

| Category | Examples |
|---|---|
| **CI/CD & source** | `gitlab`, `jenkins`, `bitbucket`, `gitea`, `gerrit`, `teamcity`, `sonarqube`, `octopus`, `spinnaker` |
| **Artifact registries** | `nexus`, `artifactory`, `harbor`, `quay`, `jfrog` |
| **Secrets & PAM** | `vault`, `cyberark`, `pvwa`, `thycotic`, `teleport`, `boundary`, `beyondtrust`, `secret-server` |
| **Identity / SSO** | `okta`, `jumpcloud`, `adfs`, `adcs`, `keycloak`, `sailpoint`, `pingfederate` |
| **Hypervisors** | `vcenter`, `esxi`, `vsphere`, `proxmox`, `hyperv`, `ovirt`, `xenserver` |
| **K8s** | `rancher`, `openshift`, `portainer`, `kubernetes-dashboard`, `k8s` |
| **Backup (DA-grade creds)** | `veeam`, `rubrik`, `cohesity`, `commvault`, `netbackup` |
| **OOB hardware** | `idrac`, `ilo`, `ipmi`, `drac`, `bmc` |
| **Logs & wikis (cred goldmines)** | `splunk`, `elastic`, `kibana`, `grafana`, `graylog`, `confluence`, `wiki`, `sharepoint`, `jira`, `servicenow` |
| **Endpoint / fleet mgmt** | `intune`, `jamf`, `sccm`, `mecm`, `wsus`, `crowdstrike`, `sentinelone` |
| **Network appliances** | `fortimanager`, `panorama`, `fmc`, `cisco-ise`, `ucs-mgr` |
| **Mail / NTLM relay** | `exchange`, `owa`, `autodiscover` |
| **Remote access** | `vpn`, `anyconnect`, `pulse-secure`, `citrix-gateway`, `rdweb` |
| **Config mgmt / IaC** | `ansible-tower`, `awx`, `puppet`, `saltmaster`, `rundeck`, `spacelift`, `terraform-enterprise` |

> **Why these specifically:** every entry on this list has one of three properties → (1) typically holds plaintext creds or LDAP binds, (2) lets you push code/binaries to other hosts, or (3) gives you administrator access to the underlying compute (hypervisor, backup, OOB, MDM). Hit one and you're often a single misconfig away from domain admin.

### `Common_list.txt` — coverage map

<details>
<summary><strong>AI coding assistants & MCP</strong> (click to expand)</summary>

`CLAUDE.md`, `AGENTS.md`, `.cursor/`, `.cursorrules`, `.windsurfrules`, `.aider.conf.yml`, `.aider.chat.history.md`, `.cline*`, `.roo*`, `.codex`, `.continue/`, `.codeium/`, `.zed/settings.json`, `.github/copilot-instructions.md`, `.mcp.json`, `claude_desktop_config.json`, `smithery.yaml`

</details>

<details>
<summary><strong>AI app builders & open-agent platforms</strong></summary>

Lovable, Base44, Wix/Velo, Bolt.new, v0.dev, Replit, OpenCode, OpenHands, LibreChat, Goose, Ollama, Jan, Msty, AnythingLLM, Open WebUI, Flowise, Dify, n8n

</details>

<details>
<summary><strong>Agent frameworks & ML ops</strong></summary>

LangGraph, LangChain, LlamaIndex, Mastra, Inngest, Trigger.dev, CrewAI, AutoGen, Letta/MemGPT, Modal, Replicate, RunPod, BentoML, MLflow, W&B, Comet

</details>

<details>
<summary><strong>Vector DBs</strong></summary>

Pinecone, Weaviate, Qdrant, Chroma, Milvus, LanceDB, Vespa, Turbopuffer

</details>

<details>
<summary><strong>2025 web frameworks & build tools</strong></summary>

TanStack Start, Solid, Qwik, Hono, Elysia, Wasp, Encore, Effect, EdgeDB, Astro, Fresh, RedwoodJS, Bun, Deno, Biome, Turbo, Nx, Rolldown, Oxc, Farm, Lightning CSS

</details>

<details>
<summary><strong>Edge / serverless / IaC</strong></summary>

Cloudflare Wrangler (`.dev.vars`, `.dev.vars.production`), Fly.io, Railway, SST v3, Pulumi (`Pulumi.production.yaml`), OpenTofu (`terraform.tfstate`), AWS CDK (`cdk.out`), Amplify Gen 2 (`amplify_outputs.json`)

</details>

<details>
<summary><strong>Modern auth & data</strong></summary>

Clerk, WorkOS, Stytch, Kinde, Logto, Authelia, Authentik, Supertokens, Better-Auth, Auth.js, Lucia, Turso, Neon, PlanetScale, Xata, libSQL, ElectricSQL, Triplit, InstantDB, Powersync, Drizzle, Convex, Supabase, Pglite

</details>

<details>
<summary><strong>Realtime / observability / security tooling</strong></summary>

Liveblocks, PartyKit, Replicache, Automerge, Yjs, OpenTelemetry, Sentry, Datadog, Honeycomb, Axiom, Highlight, PostHog, Tinybird, Trivy, Snyk, Semgrep, Gitleaks, Trufflehog, Aikido, Doppler, Infisical, Vault, sops, age

</details>

<details>
<summary><strong>CMS, testing, mobile, k8s</strong></summary>

Sanity, Payload (`payload-types.ts`), Strapi, Tina, Hygraph, Contentlayer, KeyStatic, Velite, Vitest, Playwright, Cypress, Storybook 8, Knip, Stryker, Tauri, Capacitor, Expo (`eas.json`), Helm, Kustomize, Tilt, Skaffold, Earthly, Dagger, Flux, Argo, Podman

</details>

<details>
<summary><strong>macOS dev artifacts</strong></summary>

`.fseventsd`, `.Spotlight-V100`, `.TemporaryItems`, `Info.plist`, `xcuserdata`, `Pods`, `.swiftpm`, `.icloud`, `.DocumentRevisions-V100`

</details>

<details>
<summary><strong>Internal `.md` docs (high OSINT signal)</strong></summary>

`TODO.md`, `NOTES.md`, `ROADMAP.md`, `ARCHITECTURE.md`, `RUNBOOK.md`, `SECRETS.md`, `CREDENTIALS.md`, `THREAT_MODEL.md`, `POSTMORTEM.md`, `INTERNAL.md`, `PRIVATE.md`, `STYLE.md`, `MIGRATION.md`

</details>

<details>
<summary><strong>Nuclei-templates exposures</strong></summary>

~935 paths extracted from the latest [`projectdiscovery/nuclei-templates`](https://github.com/projectdiscovery/nuclei-templates) — `http/exposures`, `http/exposed-panels`, `http/misconfiguration`, `http/files`, `http/vulnerabilities`. WordPress plugin paths, exposed admin panels, backup files, debug endpoints.

</details>

### `subdomains` — coverage map

<details>
<summary><strong>External recon — modern stack</strong></summary>

`ai`, `gpt`, `claude`, `copilot`, `gemini`, `chat-api`, `agent-api`, `mcp`, `mcp-gateway`, `prompt-studio`, `playground`, `inference`, `embeddings`, `rag`, `vector-search`, `groq`, `together`, `fireworks`, `replicate`, `modal`, `runpod`, `pinecone`, `qdrant`, `weaviate`, `chroma`, `milvus`, `clerk`, `workos`, `stytch`, `kinde`, `turso`, `neon`, `xata`, `supabase`, `convex`, `workers`, `r2`, `kv`, `d1`, `liveblocks`, `partykit`, `posthog`, `axiom`, `tinybird`, `highlight`, `cody`, `codeium`, `cursor`, `coderabbit`, `sweep`, `greptile`, `prompt-firewall`, `ai-firewall`, `mcp-firewall`, `ai-governance`, `model-cards`, `ai-bom`, `eu-ai-act`, `gpt-4o`, `o1`, `o3`, `sonnet`, `opus`, `haiku`, `llama-4`, `qwen-3`, `deepseek-r1`, `phi-4`

</details>

<details>
<summary><strong>Internal recon — corporate / on-prem</strong></summary>

`vcenter`, `esxi`, `nsx`, `idrac`, `idrac1..10`, `ilo`, `ilo1..10`, `ipmi`, `ipmi1..10`, `bmc1..10`, `kvm1..15`, `oob1..5`, `cyberark`, `pvwa`, `psm`, `cpm`, `thycotic`, `delinea`, `sailpoint`, `manageengine`, `wazuh`, `suricata`, `snort`, `zeek`, `nessus`, `qualys`, `splunk-internal`, `splunk-fwd`, `prometheus-1..2`, `grafana-1..2`, `vault-internal`, `boundary`, `teleport`, `jumpcloud`, `okta-internal`, `adfs-internal`, `dc01..03`, `ad-dc1..3`, `ldap-1..3`, `mssql-1..2`, `oracle-rac`, `mongo-1..3`, `redis-1..3`, `kafka-internal`, `rabbitmq-internal`, `harbor-1..2`, `nexus-1..2`, `artifactory-1..2`, `jenkins-1..2`, `gitlab-runner-1..2`, `veeam`, `commvault`, `rubrik`, `cohesity`, `synology-1..2`, `qnap-1..2`, `ucs-mgr`, `nx-os-internal`, `panorama`, `firepower`, `fortimanager`, `fortianalyzer`

</details>

<details>
<summary><strong>M365 / Skype-fed / hybrid mail</strong></summary>

`mysite`, `mysites`, `delve`, `viva`, `sway`, `sipfed`, `sipdir`, `sipext`, `sipinternal`, `sipgw`, `sbc`, `edgesmtp`, `oab`, `ocs`, `lyncdiscover`, `lyncweb`, `ucwa`, `mediation`, `autodiscover`, `exchange-edge`, `owa-edge`

</details>

<details>
<summary><strong>Environment / region / cluster matrix</strong></summary>

`qa1..3`, `stg1..5`, `uat1..3`, `sit1..3`, `preprod1..2`, `demo1..5`, `dr1..3`, `sandbox1..3`, `us-east-1-internal`, `eu-west-1-internal`, `ap-southeast-1-internal`, `dc-1..5`, `edge-1..20`, `pop-1..5`, `core-1..5`, `node-01..10`, `master-01..03`, `worker-01..05`, `control-plane`, `data-plane`, `mgmt-plane`

</details>

<details>
<summary><strong>Host-numeric ranges (1..30)</strong></summary>

`srv1..30`, `host1..30`, `ns1..15`, `mx1..15`, `mail1..30`, `app1..30`, `web1..30`, `vm1..30`, `relay1..20`, `lb1..20`, `proxy1..20`, `cache1..10`, `db1..30`, `ftp1..20`, `dns1..20`

</details>

<details>
<summary><strong>PoP / airport codes & locales</strong></summary>

`nyc`, `lon`, `par`, `tok`, `sgp`, `syd`, `fra`, `ams`, `hkg`, `iad`, `lax`, `sfo`, `nrt`, `icn`, `gru`, `cdg`, `lhr`, `muc`, `zrh` — plus locales: `en`, `ja`, `zh`, `ko`, `pt`, `ru`, `hi`, `nl`, `pl`, `tr`, `el`, `he`, `en-us`, `de-de`, `pt-br`, `zh-cn`, `ja-jp`

</details>

<details>
<summary><strong>Vertical-specific (academic / fintech / healthcare)</strong></summary>

Academic: `library`, `registrar`, `bursar`, `alumni`, `provost`, `eduroam`, `financial-aid`, `admissions`, `advising`, `faculty-portal`<br>
Fintech: `trading`, `fix`, `fixengine`, `bloomberg`, `reuters`, `swift-mq`, `mt4`, `mt5`, `oms`, `ems`, `order-mgmt`<br>
Healthcare: `emr`, `ehr`, `epic`, `cerner`, `meditech`, `hl7`, `fhir`

</details>

---

## Why these specific entries?

Each new entry was picked because it has a real chance of leaking one of:

1. **🔑 Secrets** — `wrangler.toml`, `.env.production.local`, `firebase-adminsdk.json`, `service-account.json`, `terraform.tfstate`
2. **🤖 Prompts & system instructions** — `CLAUDE.md`, `.cursorrules`, `system-prompt.md`, `prompts.md`
3. **🏗️ Architecture & internals** — `ARCHITECTURE.md`, `THREAT_MODEL.md`, `INTERNAL.md`, `RUNBOOK.md`, `POSTMORTEM.md`
4. **⚙️ Infrastructure config** — Pulumi configs, k8s manifests, Helm values, Wrangler bindings
5. **📦 Generated code** — `payload-types.ts`, `schema.graphql`, `generated/`, `sst-env.d.ts`
6. **🧠 Internal services** — vCenter, iDRAC/iLO, CyberArk, Wazuh, Splunk forwarders, AD/M365 federation

No wildcards, no regex, no patterns — every entry is a literal path or label, fuzz-ready as-is.

---

## Notes on case-sensitivity

The list intentionally contains both case variants for high-value files (`AGENTS.md` and `agents.md`, `CLAUDE.md` and `claude.md`). Linux web servers are case-sensitive — fuzzing only one case misses the other. Windows / IIS targets aren't affected, so you don't lose anything.

---

## Contributing

Pull requests welcome. New entries should:

- Be a **literal file or folder name / subdomain label**, not a wildcard or pattern
- Correspond to a real, currently-shipping tool, framework, or service
- Have plausible leak / discovery value (config, secrets, prompts, internals, generated code, real corp asset)
- Be checked against the existing list to avoid exact duplicates

Open a PR with a brief note on what tool / framework / vertical the entries target and roughly when it became popular.

---

## Credits

Built and maintained by [@osherassor](https://github.com/osherassor) — security researcher, pentester, CTF player.

**Companion tooling:** [LANWhisper](https://github.com/osherassor/LANWhisper) (internal DNS recon, designed to consume `subdomains` directly).

**Heritage:** classic dirbuster / RAFT / SecLists, extended with modern tooling and tradecraft those lists predate.

**License:** MIT.
