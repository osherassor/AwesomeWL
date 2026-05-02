# Default Credentials Reference

**For authorized security testing only.** This file consolidates documented vendor default credentials from public sources (SecLists, cirt.net archives, ihebski/DefaultCreds-cheat-sheet, vendor manuals, and community-maintained IoT/SCADA references). Do not use against systems you are not authorized to test.

Generated: 2026-05-02

Notes:
- `(blank)` means the field is literally empty / no password set by default.
- Where a vendor shipped multiple defaults across years/firmwares, multiple rows are listed.
- The `Notes` column captures the interface (web/SSH/Telnet/SNMP/IPMI/etc.) and whether the device prompts for a password change on first login (`must change on first login`) or keeps the default unless the operator changes it (`kept default unless changed`).
- Many seclists/cirt rows are legacy entries — verify against current firmware before relying on them.

## 1. Cameras / NVR / DVR

| Product | Vendor | Version(s) | Username | Password | Notes |
|---|---|---|---|---|---|
| Reolink IP Camera | Reolink | All | admin | (blank) | Web admin; must change on first login |
| Wansview IP Camera | Wansview | All | admin | 123456 | Web admin |
| TrendNET TV-IP Camera | TrendNET | All | admin | admin | Web admin |
| Lorex DVR/NVR | Lorex | All | admin | 000000 | Web admin (Dahua OEM) |
| Swann DVR | Swann | All | admin | 12345 | Web/RTSP |
| Foscam IP Camera | Foscam | All | admin | (blank) | Web admin |
| ACTi IP Camera | ACTi | All | Admin | 123456 | Web admin |
| GeoVision DVR/NVR | GeoVision | All | admin | admin | Web admin/RTSP |
| Vivotek IP Camera | Vivotek | All | root | (blank) | Web admin; must set password on first access |
| Pelco Sarix / Spectra | Pelco | All | admin | admin | Web admin |
| Bosch Divar IP NVR | Bosch | All | BVRAdmin | WSS4Bosch | OS admin; kept default unless changed |
| AXIS Network Camera | Axis | >=5.20 | root | (blank) | Must set on first access; web admin |
| Dahua DSS Pro/Express | Dahua | All | system | system | Management server |
| DS-Series IP Camera/NVR | Hikvision | All (pre-2014 firmware) | admin | 12345 | Web/RTSP/SDK; CVE-2017-7921; kept default unless changed |
| Actiontec | Actiontec | All | (blank) | (blank) | From SecLists/cirt.net archive |
| Actiontec | Actiontec | All | admin | password | Verizon Fios Setup |
| Audioactive | Audioactive | All | (blank) | telos | From SecLists/cirt.net archive |
| Axis | Axis | All | <N/A> | (blank) | From SecLists/cirt.net archive |
| Axis Communications | Axis Communications | All | root | pass | From SecLists/cirt.net archive |
| Axis | Axis | All | root | pass | From SecLists/cirt.net archive |
| Best Practical Solutions | Best Practical Solutions | All | root | password | http://requesttracker.wikia.com/wiki/RecoverRootPassword |
| BestPractical | BestPractical | All | root | password | From SecLists/cirt.net archive |
| Bosch | Bosch | All | live | live | From SecLists/cirt.net archive |
| Bosch | Bosch | All | service | service | From SecLists/cirt.net archive |
| Bosch | Bosch | All | user | user | From SecLists/cirt.net archive |
| Foscam | Foscam | All | admin | (blank) | http://foscam.com/Private/ProductFiles/FI8918W%20user%20manual-v36.00.pdf |
| Galacticomm | Galacticomm | All | Sysop | Sysop | From SecLists/cirt.net archive |
| Hikvision Network Camera | Hikvision Network Camera | All | admin | 12345 | https://www.hikvision.com/UploadFile/image/EN-user%20manual%20of%20%20network%20camera%20v3.0.0.pdf |
| IQinVision | IQinVision | All | root | system | http://www.iqeye.com/iqeye/images/uploads/File/manuals/Quick-Install.pdf |
| Mercury Interactive | Mercury Interactive | All | admin | admin | From SecLists/cirt.net archive |
| Mobotix | Mobotix | All | admin | meinsm | From SecLists/cirt.net archive |
| Site Interactive | Site Interactive | All | admin | pass | From SecLists/cirt.net archive |
| actiontec | actiontec | All | admin | admin | From SecLists/cirt.net archive |
| ActiveMQ (general) | ActiveMQ (general) | All | admin | admin | From SecLists/cirt.net archive |
| ActiveMQ (general) | ActiveMQ (general) | All | (blank) | (blank) | From SecLists/cirt.net archive |
| acti (web) | acti (web) | All | admin | 12345 | From SecLists/cirt.net archive |
| acti (web) | acti (web) | All | admin | 123456 | From SecLists/cirt.net archive |
| Amcrest | Amcrest | All | admin | admin | From SecLists/cirt.net archive |
| American Dynamics EDVR (telnet) | American Dynamics EDVR (telnet) | All | admin | 9999 | From SecLists/cirt.net archive |
| Apache Axis2 | Apache Axis2 | All | admin | axis2 | From SecLists/cirt.net archive |
| Axis | Axis | All | (blank) | (blank) | From SecLists/cirt.net archive |
| Axis camera (web) | Axis camera (web) | All | root | (blank) | From SecLists/cirt.net archive |
| Axis (web) | Axis (web) | All | root | admin | From SecLists/cirt.net archive |
| Axis (web) | Axis (web) | All | root | pass | From SecLists/cirt.net archive |
| Axis (web) | Axis (web) | All | root | root | From SecLists/cirt.net archive |
| Bosch | Bosch | All | (blank) | (blank) | From SecLists/cirt.net archive |
| Bosch RPS (mssql) | Bosch RPS (mssql) | All | sa | RPSsql12345 | From SecLists/cirt.net archive |
| Cacti (web) | Cacti (web) | All | admin | admin | From SecLists/cirt.net archive |
| Dahua | Dahua | All | admin | admin | From SecLists/cirt.net archive |
| FLIR (Dahua OEM) | FLIR (Dahua OEM) | All | admin | admin | From SecLists/cirt.net archive |
| geovision (web) | geovision (web) | All | admin | admin | From SecLists/cirt.net archive |
| hikvision (ssh) | hikvision (ssh) | All | admin | 12345 | From SecLists/cirt.net archive |
| icatch (camera) | icatch (camera) | All | admin | 123456 | From SecLists/cirt.net archive |
| icatch (camera) | icatch (camera) | All | root | icatch99 | From SecLists/cirt.net archive |
| IP camera 5 Mpix DA-IP8517TDV (analog DONGJIA DJ-IPC-HD8517TDV) (telnet) | IP camera 5 Mpix DA-IP8517TDV (analog DONGJIA DJ-IPC-HD8517TDV) (telnet) | All | root | tl789 | From SecLists/cirt.net archive |
| IP camera a5s66_imx322 (telnet) | IP camera a5s66_imx322 (telnet) | All | root | h2014071 | From SecLists/cirt.net archive |
| IP camera Hi3515 (telnet) | IP camera Hi3515 (telnet) | All | root | xc3511 | From SecLists/cirt.net archive |
| IP camera Hi3516 sensor imx122 (telnet) | IP camera Hi3516 sensor imx122 (telnet) | All | root | cat1029 | From SecLists/cirt.net archive |
| IP camera HI3516 (telnet) | IP camera HI3516 (telnet) | All | root | xmhdipc | From SecLists/cirt.net archive |
| IP camera Hi3518E (telnet) | IP camera Hi3518E (telnet) | All | root | xmhdipc | From SecLists/cirt.net archive |
| IP camera NVR SunEyes (HD-Network Real-time) (telnet) | IP camera NVR SunEyes (HD-Network Real-time) (telnet) | All | root | antslq | From SecLists/cirt.net archive |
| IP camera (Remote MGMT) (telnet) | IP camera (Remote MGMT) (telnet) | All | root | jvbzd | From SecLists/cirt.net archive |
| IP camera SMTSEC IMX185+Hi3516A_2Mp_1080p_H.265 (telnet) | IP camera SMTSEC IMX185+Hi3516A_2Mp_1080p_H.265 (telnet) | All | root | fxjvt1805 | From SecLists/cirt.net archive |
| IP camera VC-A20IPBLF1 (HI3516C_IMX322) (telnet) | IP camera VC-A20IPBLF1 (HI3516C_IMX322) (telnet) | All | adminlvjh | adminlvjh123 | From SecLists/cirt.net archive |
| IP camera VC-A20IPBLF1 (HI3516C_IMX322) (telnet) | IP camera VC-A20IPBLF1 (HI3516C_IMX322) (telnet) | All | root | HI1602014x | From SecLists/cirt.net archive |
| IP camera ПМ-005-IP-E-COS24-25 (telnet) | IP camera ПМ-005-IP-E-COS24-25 (telnet) | All | adminlvjh | adminlvjh123 | From SecLists/cirt.net archive |
| iqinvision (web) | iqinvision (web) | All | root | system | From SecLists/cirt.net archive |
| Longse (IP camera) | Longse (IP camera) | All | admin | 12345 | From SecLists/cirt.net archive |
| Lorex | Lorex | All | admin | admin | From SecLists/cirt.net archive |
| LTS (IP camera) | LTS (IP camera) | All | admin | 12345 | From SecLists/cirt.net archive |
| March Networks (IP camera) | March Networks (IP camera) | All | admin | (blank) | From SecLists/cirt.net archive |
| MayGion Camera (webcam) | MayGion Camera (webcam) | All | admin | admin | From SecLists/cirt.net archive |
| mobotix (web) | mobotix (web) | All | admin | meinsm | From SecLists/cirt.net archive |
| Northern (IP camera) | Northern (IP camera) | All | admin | 12345 | From SecLists/cirt.net archive |
| Oncam (IP camera) | Oncam (IP camera) | All | admin | admin | From SecLists/cirt.net archive |
| Pelco DS Admin / DS ControlPoint | Pelco DS Admin / DS ControlPoint | All | admin | admin | From SecLists/cirt.net archive |
| Pelco DS Services | Pelco DS Services | All | DSNVSUser | Pelco123 | From SecLists/cirt.net archive |
| Pelco DS SQL (v7.x.x) | Pelco DS SQL (v7.x.x) | All | sa | LETmein333 | From SecLists/cirt.net archive |
| Pelco DS Windows Login (DIACAP DS version 7.14) | Pelco DS Windows Login (DIACAP DS version 7.14) | All | DSServiceUser | Q2_Pelco@$2016 | From SecLists/cirt.net archive |
| Pelco DS Windows Login (DIACAP DS version 7.16) | Pelco DS Windows Login (DIACAP DS version 7.16) | All | DSServiceUser | Q1_17@$Pelc0DS | From SecLists/cirt.net archive |
| Pelco DS Windows Login (DIACAP DS version 7.7) | Pelco DS Windows Login (DIACAP DS version 7.7) | All | DSServiceUser | ds_Pelco@$2014 | From SecLists/cirt.net archive |
| Pelco DS Windows Login | Pelco DS Windows Login | All | DSServiceUser | dsserviceuser | From SecLists/cirt.net archive |
| Pelco DVXi / DVXe | Pelco DVXi / DVXe | All | Administrator | letmein | From SecLists/cirt.net archive |
| Pelco DX1000 | Pelco DX1000 | All | (blank) | 000 or 202 | From SecLists/cirt.net archive |
| Pelco DX3100 Server | Pelco DX3100 Server | All | (blank) | 1981 | From SecLists/cirt.net archive |
| Pelco DX4000 Server | Pelco DX4000 Server | All | (blank) | 1234 | From SecLists/cirt.net archive |
| Pelco DX4500 / DX4600 Client | Pelco DX4500 / DX4600 Client | All | (blank) | 000000 | From SecLists/cirt.net archive |
| Pelco DX4500 / DX4600 Server (Firmware 1.2 or older) | Pelco DX4500 / DX4600 Server (Firmware 1.2 or older) | All | ADMINISTRATOR | 000000 | From SecLists/cirt.net archive |
| Pelco DX4500 / DX4600 Server (Firmware 1.3 or newer) | Pelco DX4500 / DX4600 Server (Firmware 1.3 or newer) | All | admin | admin | From SecLists/cirt.net archive |
| Pelco DX8100 Client | Pelco DX8100 Client | All | (blank) | 000000 | From SecLists/cirt.net archive |
| Pelco DX8100 Server v1.x  (Prompts to change password on 1st login) | Pelco DX8100 Server v1.x  (Prompts to change password on 1st login) | All | Admin | Admin | From SecLists/cirt.net archive |
| Pelco DX8100 Server v2.x (Prompts to change but can keep default) | Pelco DX8100 Server v2.x (Prompts to change but can keep default) | All | admin | admin | From SecLists/cirt.net archive |
| Pelco DX8100 Server Windows Login Exit to Windows | Pelco DX8100 Server Windows Login Exit to Windows | All | dx8100adm | dx8100 | From SecLists/cirt.net archive |
| Pelco Endura SSH (SM5000/SM5200/NSM5200/VCD5000/VCD5202/NET5402R-HD/UDI5000-CAM/UDI5000-MTRX) | Pelco Endura SSH (SM5000/SM5200/NSM5200/VCD5000/VCD5202/NET5402R-HD/UDI5000-CAM/UDI5000-MTRX) | All | root | pel2899100 | From SecLists/cirt.net archive |
| Pelco Endura Web Interface (SM5000/SM5200/NSM520) | Pelco Endura Web Interface (SM5000/SM5200/NSM520) | All | admin | admin | From SecLists/cirt.net archive |
| Pelco Endura Windows Login (WS5050/WS5060/WS5070/WS5080) | Pelco Endura Windows Login (WS5050/WS5060/WS5070/WS5080) | All | WS50x0 Administrator (Substitute the x with the model of the workstation) | 2899100 | From SecLists/cirt.net archive |
| Pelco Endura WS5200 Software | Pelco Endura WS5200 Software | All | admin | admin | From SecLists/cirt.net archive |
| Pelco Sarix SSH | Pelco Sarix SSH | All | root | pel2899100 | From SecLists/cirt.net archive |
| Pelco Sarix Web Interface | Pelco Sarix Web Interface | All | admin | admin | From SecLists/cirt.net archive |
| Pelco VideoXpert Accessory Server SSH | Pelco VideoXpert Accessory Server SSH | All | pelco | Pel2899100 | From SecLists/cirt.net archive |
| Pelco VideoXpert Accessory Server Webpage (v2.0+) | Pelco VideoXpert Accessory Server Webpage (v2.0+) | All | admin | admin | From SecLists/cirt.net archive |
| Pelco VideoXpert Admin Portal (This must be changed upon initial configuration) | Pelco VideoXpert Admin Portal (This must be changed upon initial configuration) | All | admin | admin | From SecLists/cirt.net archive |
| Pelco VideoXpert Enhanced Decoder SSH | Pelco VideoXpert Enhanced Decoder SSH | All | decoder | pelco | From SecLists/cirt.net archive |
| Pelco VideoXpert OpsCenter Local Credentials | Pelco VideoXpert OpsCenter Local Credentials | All | localadmin | localadmin | From SecLists/cirt.net archive |
| Pelco VideoXpert Storage Server Webpage | Pelco VideoXpert Storage Server Webpage | All | admin | admin | From SecLists/cirt.net archive |
| Pelco VideoXpert Storage Server Webpage (Updated) | Pelco VideoXpert Storage Server Webpage (Updated) | All | admin | Pel2899100 | From SecLists/cirt.net archive |
| Pelco VideoXpert Windows Login | Pelco VideoXpert Windows Login | All | pelco | Pel2899100 | From SecLists/cirt.net archive |
| Q-See (IPcamera) | Q-See (IPcamera) | All | admin | 123456 | From SecLists/cirt.net archive |
| Q-See (IP camera) | Q-See (IP camera) | All | admin | admin | From SecLists/cirt.net archive |
| Reolink (IP camera) | Reolink (IP camera) | All | admin | (blank) | From SecLists/cirt.net archive |
| Samsung Electronics (IP camera) | Samsung Electronics (IP camera) | All | admin | 4321 | From SecLists/cirt.net archive |
| Samsung Electronics (IP camera) | Samsung Electronics (IP camera) | All | root | root | From SecLists/cirt.net archive |
| Samsung Techwin (IP camera) | Samsung Techwin (IP camera) | All | admin | 1111111 | From SecLists/cirt.net archive |
| Sanyo (IP camera) | Sanyo (IP camera) | All | admin | admin | From SecLists/cirt.net archive |
| Scallop (IP camera) | Scallop (IP camera) | All | admin | password | From SecLists/cirt.net archive |
| Speco Technologies IP Camera (camera) | Speco Technologies IP Camera (camera) | All | admin | 1234 | From SecLists/cirt.net archive |
| Starvedia (IP camera) | Starvedia (IP camera) | All | admin | (blank) | From SecLists/cirt.net archive |
| Sunell (IP camera) | Sunell (IP camera) | All | admin | admin | From SecLists/cirt.net archive |
| SV3C (IP camera) | SV3C (IP camera) | All | admin | 123456 | From SecLists/cirt.net archive |
| Swann (IP-cam) | Swann (IP-cam) | All | admin | 12345 | From SecLists/cirt.net archive |
| Swann (IP camera) | Swann (IP camera) | All | admin | 12345 | From SecLists/cirt.net archive |
| Toshiba (IP camera) | Toshiba (IP camera) | All | root | ikwd | From SecLists/cirt.net archive |
| TRENDnet Internet Camera (webcam) | TRENDnet Internet Camera (webcam) | All | admin | admin | From SecLists/cirt.net archive |
| Vivotek (IP camera) | Vivotek (IP camera) | All | root | (blank) | From SecLists/cirt.net archive |
| Vivotek (IP-cam) | Vivotek (IP-cam) | All | root | (blank) | From SecLists/cirt.net archive |
| W-Box (Hikvision OEM old) (IP-cam) | W-Box (Hikvision OEM old) (IP-cam) | All | admin | wbox123 | From SecLists/cirt.net archive |
| W-Box (Hikvision OEM old) (IP camera) | W-Box (Hikvision OEM old) (IP camera) | All | admin | wbox123 | From SecLists/cirt.net archive |
| W-Box (Sunell OEM new) (IP camera) | W-Box (Sunell OEM new) (IP camera) | All | admin | admin | From SecLists/cirt.net archive |

## 2. Printers / MFPs

| Product | Vendor | Version(s) | Username | Password | Notes |
|---|---|---|---|---|---|
| OKI MC/MB series | OKI | All | root | (blank) | Web admin |
| OKI MC/MB series | OKI | All | admin | aaaaaa | Web admin |
| bizhub C-series | Konica Minolta | All | admin | 12345678 | Web admin |
| Aficio MP supervisor | Ricoh | All | supervisor | (blank) | Web Image Monitor supervisor |
| Aficio MP | Ricoh | All | admin | (blank) | Web Image Monitor; kept default unless changed |
| Lexmark MX/MS series | Lexmark | All | admin | (blank) | Web admin |
| ImageRunner ADVANCE | Canon | All | 7654321 | 7654321 | Service mode |
| ImageRunner ADVANCE | Canon | All | ADMIN | (blank) | Remote UI; kept default unless changed |
| LaserJet/JetDirect EWS | HP | All | (blank) | (blank) | Default has no auth; admin must enable |
| LaserJet 4000/4050/4100 series | HP | All | admin | (blank) | Web JetAdmin/EWS; kept default unless changed |
| Brother | Brother | All | (blank) | access | From SecLists/cirt.net archive |
| Brother | Brother | All | <N/A> | access | From SecLists/cirt.net archive |
| Brother Industries Ltd. | Brother Industries Ltd. | All | (blank) | 00000000 | From SecLists/cirt.net archive |
| Brother Industries Ltd. | Brother Industries Ltd. | All | (blank) | 12345678 | From SecLists/cirt.net archive |
| Brother Industries Ltd. | Brother Industries Ltd. | All | admin | access | From SecLists/cirt.net archive |
| Brother | Brother | All | admin | access | From SecLists/cirt.net archive |
| Canon/Brother | Canon/Brother | All | 7654321 | 7654321 | From SecLists/cirt.net archive |
| Canon | Canon | All | <N/A> | 0 | From SecLists/cirt.net archive |
| Hewlett Packard | Hewlett Packard | All | admin | admin | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | (blank) | (blank) | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | (blank) | hewlpack | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | <N/A> | hewlpack | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | ADVMAIL | (blank) | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | ADVMAIL | HP | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | ADVMAIL | HPOFFICE DATA | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | Admin | Admin | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | Administrator | The last eight digits of the serial number | http://bizsupport1.austin.hp.com/bizsupport/TechSupport/Document.jsp?objectID=c01141537&lang=en&cc=us&taskId=101&prodSeriesId=428936&prodTypeId=15351 |
| Hewlett-Packard | Hewlett-Packard | All | Anonymous | (blank) | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | FIELD | (blank) | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | FIELD | HPONLY | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | FIELD | HPP187 SYS | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | FIELD | HPWORD PUB | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | FIELD | LOTUS | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | FIELD | MANAGER | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | FIELD | MGR | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | FIELD | SERVICE | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | FIELD | SUPPORT | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | HELLO | FIELD.SUPPORT | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | HELLO | MANAGER.SYS | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | HELLO | MGR.SYS | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | HELLO | OP.OPERATOR | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | HPSupport | badg3r5 | http://www.lolware.net/hpstorage.html |
| Hewlett-Packard | Hewlett-Packard | All | MAIL | HPOFFICE | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | MAIL | MAIL | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | MAIL | MPE | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | MAIL | REMOTE | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | MAIL | TELESUP | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | MANAGER | COGNOS | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | MANAGER | HPOFFICE | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | MANAGER | ITF3000 | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | MANAGER | SECURITY | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | MANAGER | SYS | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | MANAGER | TCH | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | MANAGER | TELESUP | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | MGE | VESOFT | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | MGR | CAROLIAN | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | MGR | CCC | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | MGR | CNAS | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | MGR | COGNOS | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | MGR | CONV | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | MGR | HPDESK | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | MGR | HPOFFICE | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | MGR | HPONLY | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | MGR | HPP187 | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | MGR | HPP189 | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | MGR | HPP196 | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | MGR | INTX3 | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | MGR | ITF3000 | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | MGR | NETBASE | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | MGR | REGO | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | MGR | RJE | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | MGR | ROBELLE | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | MGR | SECURITY | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | MGR | SYS | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | MGR | TELESUP | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | MGR | VESOFT | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | MGR | WORD | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | MGR | XLSERVER | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | OPERATOR | COGNOS | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | OPERATOR | DISC | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | OPERATOR | SUPPORT | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | OPERATOR | SYS | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | OPERATOR | SYSTEM | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | Oper | Oper | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | PCUSER | SYS | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | RSBCMON | SYS | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | SPOOLMAN | HPOFFICE | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | WP | HPOFFICE | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | admin | hp.com | From SecLists/cirt.net archive |
| Hewlett-Packard | Hewlett-Packard | All | admin | isee | From SecLists/cirt.net archive |
| Konica Minolta | Konica Minolta | All | (blank) | 0000 | From SecLists/cirt.net archive |
| Konica Minolta | Konica Minolta | All | (blank) | 1234 | From SecLists/cirt.net archive |
| Konica Minolta | Konica Minolta | All | (blank) | (blank) | From SecLists/cirt.net archive |
| Konica Minolta | Konica Minolta | All | (blank) | MagiMFP | http://www.kn.nl/data/handleiding/182185/Reference%20Guide%20Magicolor%202490MF.pdf |
| Konica Minolta | Konica Minolta | All | (blank) | sysAdmin | From SecLists/cirt.net archive |
| Konica Minolta | Konica Minolta | All | <N/A> | 0 | Printer configuration interface |
| Konica Minolta | Konica Minolta | All | <N/A> | sysadm | From SecLists/cirt.net archive |
| Konica Minolta | Konica Minolta | All | admin | administrator | From SecLists/cirt.net archive |
| Kyocera | Kyocera | All | 2800 | 2800 | From SecLists/cirt.net archive |
| Kyocera | Kyocera | All | (blank) | admin00 | From SecLists/cirt.net archive |
| Kyocera | Kyocera | All | <N/A> | PASSWORD | From SecLists/cirt.net archive |
| Kyocera | Kyocera | All | <N/A> | admin00 | From SecLists/cirt.net archive |
| Kyocera | Kyocera | All | admin | (blank) | From SecLists/cirt.net archive |
| Kyocera | Kyocera | All | admin | admin | From SecLists/cirt.net archive |
| Kyocera | Kyocera | All | root | root | From SecLists/cirt.net archive |
| Minolta PagrPro | Minolta PagrPro | All | <N/A> | sysadm | From SecLists/cirt.net archive |
| Minolta QMS | Minolta QMS | All | admin | (blank) | From SecLists/cirt.net archive |
| Minolta QMS | Minolta QMS | All | operator | (blank) | From SecLists/cirt.net archive |
| NRG or RICOH | NRG or RICOH | All | (blank) | password | From SecLists/cirt.net archive |
| Nokia | Nokia | All | (blank) | 9999 | From SecLists/cirt.net archive |
| Nokia | Nokia | All | (blank) | Telecom | From SecLists/cirt.net archive |
| Nokia | Nokia | All | (blank) | nokai | From SecLists/cirt.net archive |
| Nokia | Nokia | All | (blank) | nokia | From SecLists/cirt.net archive |
| Nokia | Nokia | All | Security Code | 12345 | From SecLists/cirt.net archive |
| Nokia | Nokia | All | Telecom | Telecom | From SecLists/cirt.net archive |
| Nokia | Nokia | All | client | client | From SecLists/cirt.net archive |
| Nokia | Nokia | All | m1122 | m1122 | From SecLists/cirt.net archive |
| Nokia | Nokia | All | nop | 12345 | From SecLists/cirt.net archive |
| Nokia | Nokia | All | nop | 123454 | From SecLists/cirt.net archive |
| Nokia | Nokia | All | root | nokia | From SecLists/cirt.net archive |
| Nokia | Nokia | All | root | rootme | From SecLists/cirt.net archive |
| Oki | Oki | All | admin | <SEE COMMENT> | Last 6 characters of the MAC address in uppercase |
| Oki | Oki | All | admin | OkiLAN | From SecLists/cirt.net archive |
| Oki | Oki | All | root | <SEE COMMENT> | Last 6 characters of the MAC address in uppercase |
| Ricoh | Ricoh | All | (blank) | password | From SecLists/cirt.net archive |
| Ricoh | Ricoh | All | (blank) | sysadm | From SecLists/cirt.net archive |
| Ricoh | Ricoh | All | <N/A> | password | From SecLists/cirt.net archive |
| Ricoh | Ricoh | All | <N/A> | sysadm | From SecLists/cirt.net archive |
| Ricoh | Ricoh | All | admin | (blank) | From SecLists/cirt.net archive |
| Ricoh | Ricoh | All | admin | no password | From SecLists/cirt.net archive |
| Ricoh | Ricoh | All | admin | password | From SecLists/cirt.net archive |
| Ricoh | Ricoh | All | sysadm | sysadm | From SecLists/cirt.net archive |
| Ricoh | Ricoh | All | sysadmin | password | From SecLists/cirt.net archive |
| Sharp | Sharp | All | <N/A> | sysadm | From SecLists/cirt.net archive |
| Sharp | Sharp | All | Administrator | admin | From SecLists/cirt.net archive |
| Sharp | Sharp | All | admin | Sharp | From SecLists/cirt.net archive |
| Sharp | Sharp | All | admin | admin | Different to other Sharp units |
| Sharp | Sharp | All | (blank) | sysadm | From SecLists/cirt.net archive |
| Toshiba | Toshiba | All | (blank) | 24Banc81 | From SecLists/cirt.net archive |
| Toshiba | Toshiba | All | (blank) | Toshiba | From SecLists/cirt.net archive |
| Toshiba | Toshiba | All | (blank) | toshy99 | From SecLists/cirt.net archive |
| Toshiba | Toshiba | All | <N/A> | 24Banc81 | From SecLists/cirt.net archive |
| Toshiba | Toshiba | All | <N/A> | (blank) | From SecLists/cirt.net archive |
| Toshiba | Toshiba | All | <N/A> | Toshiba | From SecLists/cirt.net archive |
| Toshiba | Toshiba | All | <N/A> | toshy99 | From SecLists/cirt.net archive |
| Toshiba | Toshiba | All | Admin | 123456 | From SecLists/cirt.net archive |
| Toshiba | Toshiba | All | super | superpass | From SecLists/cirt.net archive |
| Xerox | Xerox | All | 11111 | x-admin | From SecLists/cirt.net archive |
| Xerox | Xerox | All | (blank) | 11111 | From SecLists/cirt.net archive |
| Xerox | Xerox | All | <N/A> | 0 | From SecLists/cirt.net archive |
| Xerox | Xerox | All | Administrator | Fiery.1 | From SecLists/cirt.net archive |
| Xerox | Xerox | All | NSA | nsa | http://download.support.xerox.com/pub/docs/FlowPort2/userdocs/any-os/en/fp_dc_setup_guide.pdf |
| Xerox | Xerox | All | admin | 1111 | From SecLists/cirt.net archive |
| Xerox | Xerox | All | admin | 2222 | From SecLists/cirt.net archive |
| Xerox | Xerox | All | admin | 22222 | works for access panel 2 |
| Xerox | Xerox | All | admin | (blank) | From SecLists/cirt.net archive |
| Xerox | Xerox | All | admin | admin | From SecLists/cirt.net archive |
| Xerox | Xerox | All | admin | x-admin | From SecLists/cirt.net archive |
| Xerox | Xerox | All | savelogs | crash | From SecLists/cirt.net archive |
| sharp | sharp | All | <N/A> | (blank) | From SecLists/cirt.net archive |
| xerox | xerox | All | <N/A> | admin | From SecLists/cirt.net archive |
| Brother HL Series (printer) | Brother HL Series (printer) | All | admin | access | From SecLists/cirt.net archive |
| Brother Printer (web) | Brother Printer (web) | All | admin | access | From SecLists/cirt.net archive |
| Canon | Canon | All | Administrator | 7654321 | From SecLists/cirt.net archive |
| Canon | Canon | All | (blank) | 0 | From SecLists/cirt.net archive |
| Canon Printer (web) | Canon Printer (web) | All | ADMIN | canon | From SecLists/cirt.net archive |
| canon (web) | canon (web) | All | root | camera | From SecLists/cirt.net archive |
| EPSON | EPSON | All | EPSONWEB | admin | From SecLists/cirt.net archive |
| Epson Printer (web) | Epson Printer (web) | All | EPSONWEB | admin | From SecLists/cirt.net archive |
| Hewlett Packard Enterprise BMC | Hewlett Packard Enterprise BMC | All | admin | admin | From SecLists/cirt.net archive |
| Hewlett Packard - Storage Management Utility (SMU) [<VE270P003/VL270P003] (FTP) | Hewlett Packard - Storage Management Utility (SMU) [<VE270P003/VL270P003] (FTP) | All | ftp | !ftp | From SecLists/cirt.net archive |
| Hewlett Packard - Storage Management Utility (SMU) [>VE270P003/VL270P003] (WEB ) | Hewlett Packard - Storage Management Utility (SMU) [>VE270P003/VL270P003] (WEB ) | All | setup | (blank) | From SecLists/cirt.net archive |
| Hewlett Packard - Storage Management Utility (SMU) [<VE270P003/VL270P003] (WEB: View and change) | Hewlett Packard - Storage Management Utility (SMU) [<VE270P003/VL270P003] (WEB: View and change) | All | manage | !manage | From SecLists/cirt.net archive |
| Hewlett Packard - Storage Management Utility (SMU) [<VE270P003/VL270P003] (WEB: View only) | Hewlett Packard - Storage Management Utility (SMU) [<VE270P003/VL270P003] (WEB: View only) | All | monitor | !monitor | From SecLists/cirt.net archive |
| HP iLO (IPMI) | HP iLO (IPMI) | All | admin | admin | From SecLists/cirt.net archive |
| HP iLO (IPMI) | HP iLO (IPMI) | All | admin | <random string 8 symbol> | From SecLists/cirt.net archive |
| HP LaserJet 600 (printer) | HP LaserJet 600 (printer) | All | (blank) | (blank) | From SecLists/cirt.net archive |
| HP LaserJet No Password Legacy (printer) | HP LaserJet No Password Legacy (printer) | All | (blank) | (blank) | From SecLists/cirt.net archive |
| HP LaserJet No Password (printer) | HP LaserJet No Password (printer) | All | (blank) | (blank) | From SecLists/cirt.net archive |
| HP Server Automation (web) | HP Server Automation (web) | All | Administrator | admin | From SecLists/cirt.net archive |
| HP Server Automation (web) | HP Server Automation (web) | All | admin | opsware_admin | From SecLists/cirt.net archive |
| HP StoreAll (GUI) | HP StoreAll (GUI) | All | ibrix | ibrix | From SecLists/cirt.net archive |
| HP StoreAll (Root) | HP StoreAll (Root) | All | root | hpinvent | From SecLists/cirt.net archive |
| Konica Minolta | Konica Minolta | All | (blank) | 0 | From SecLists/cirt.net archive |
| Konica Minolta | Konica Minolta | All | (blank) | 1234567812345678 | From SecLists/cirt.net archive |
| Konica Minolta | Konica Minolta | All | (blank) | sysadm | From SecLists/cirt.net archive |
| Konica Minolta (web) | Konica Minolta (web) | All | admin | administrator | From SecLists/cirt.net archive |
| Konica Minolta (web) | Konica Minolta (web) | All | (blank) | 0 | From SecLists/cirt.net archive |
| Konica Minolta (web) | Konica Minolta (web) | All | (blank) | 0000 | From SecLists/cirt.net archive |
| Konica Minolta (web) | Konica Minolta (web) | All | (blank) | 1234 | From SecLists/cirt.net archive |
| Konica Minolta (web) | Konica Minolta (web) | All | (blank) | 1234567812345678 | From SecLists/cirt.net archive |
| Konica Minolta (web) | Konica Minolta (web) | All | (blank) | (blank) | From SecLists/cirt.net archive |
| Konica Minolta (web) | Konica Minolta (web) | All | (blank) | MagiMFP | From SecLists/cirt.net archive |
| Konica Minolta (web) | Konica Minolta (web) | All | (blank) | sysadm | From SecLists/cirt.net archive |
| Konica Minolta (web) | Konica Minolta (web) | All | (blank) | sysAdmin | From SecLists/cirt.net archive |
| Kyocera | Kyocera | All | (blank) | PASSWORD | From SecLists/cirt.net archive |
| Lexmark Printer (web) | Lexmark Printer (web) | All | admin | (blank) | From SecLists/cirt.net archive |
| Minolta PagrPro | Minolta PagrPro | All | (blank) | sysadm | From SecLists/cirt.net archive |
| Nokia G-140W-C | Nokia G-140W-C | All | AdminGPON | ALC@#FGU | From SecLists/cirt.net archive |
| Ricoh MP (printer) | Ricoh MP (printer) | All | supervisor | (blank) | From SecLists/cirt.net archive |
| Ricoh Printer | Ricoh Printer | All | admin | (blank) | From SecLists/cirt.net archive |
| sharp | sharp | All | (blank) | (blank) | From SecLists/cirt.net archive |
| Sharp | Sharp | All | (blank) | sysadm | From SecLists/cirt.net archive |
| Sharp Printer (web) | Sharp Printer (web) | All | admin | Sharp | From SecLists/cirt.net archive |
| Toshiba | Toshiba | All | (blank) | (blank) | From SecLists/cirt.net archive |
| Toshiba (IP-cam) | Toshiba (IP-cam) | All | root | ikwd | From SecLists/cirt.net archive |
| Xerox | Xerox | All | (blank) | 0 | From SecLists/cirt.net archive |
| xerox | xerox | All | (blank) | admin | From SecLists/cirt.net archive |
| XEROX Phaser 6700 (printer) | XEROX Phaser 6700 (printer) | All | admin | 1111 | From SecLists/cirt.net archive |
| Xerox WorkCentre 5020/DN (printer) | Xerox WorkCentre 5020/DN (printer) | All | 11111 | (blank) | From SecLists/cirt.net archive |

## 3. Networking — routers / switches / firewalls

| Product | Vendor | Version(s) | Username | Password | Notes |
|---|---|---|---|---|---|
| Pulse Secure / Ivanti Connect | Pulse Secure | All | admin | (set on install) | Web admin |
| NetScaler ADC/Gateway | Citrix | All | nsroot | nsroot | Web/SSH; must change on first login |
| BIG-IP root | F5 | All | root | default | SSH; must change on first login |
| BIG-IP | F5 | All | admin | admin | Web/SSH; must change on first login |
| 3Com SuperStack | 3Com | All | admin | (blank) | Web/Telnet |
| AsusWRT | Asus | All | admin | admin | Web admin; must change on first login |
| Buffalo AirStation | Buffalo | All | root | (blank) | Web admin |
| ZTE H-series CPE | ZTE | All | admin | admin | Web admin |
| Huawei AR/S-series | Huawei | All | admin | Admin@huawei | Web/SSH; must change on first login |
| Sophos UTM/XG | Sophos | All | admin | (set on install) | Set during install; no shipped default |
| Linksys WRT-series | Linksys | All | (blank) | admin | Web admin |
| Archer/Deco | TP-Link | Newer | (blank) | (blank) | Set on first login via web/app |
| DIR-series router | D-Link | All | admin | (blank) | Web admin |
| ArubaOS controller | Aruba | All | admin | (blank) | CLI/web; must set |
| EdgeOS / EdgeRouter | Ubiquiti | All | ubnt | ubnt | SSH/web admin |
| RouterOS | MikroTik | <6.49 | admin | (blank) | Winbox/SSH/web; newer ship without password requiring console set |
| PAN-OS firewall | Palo Alto | All | admin | admin | Web admin; must change on first login |
| FortiGate | Fortinet | <5.4 | admin | (blank) | Web/SSH; must change on first login (newer) |
| Junos OS | Juniper | All | root | (blank) | CLI; must set on first commit |
| Meraki MX/MS/MR (cloud) | Cisco Meraki | All | (blank) | (blank) | Cloud-managed; no local default; must register |
| Cisco DPC3825/EPC3825 modem | Cisco | All | admin | password | Web admin |
| ASA / PIX | Cisco | All | (blank) | cisco | Enable; web ASDM admin/(blank) |
| 3COM | 3COM | All | 3comcso | RIP000 | Resets all passwords to defaults |
| 3COM | 3COM | All | (blank) | 12345 | From SecLists/cirt.net archive |
| 3COM | 3COM | All | (blank) | 1234admin | From SecLists/cirt.net archive |
| 3COM | 3COM | All | (blank) | (blank) | From SecLists/cirt.net archive |
| 3COM | 3COM | All | (blank) | ANYCOM | From SecLists/cirt.net archive |
| 3COM | 3COM | All | (blank) | ILMI | From SecLists/cirt.net archive |
| 3COM | 3COM | All | (blank) | PASSWORD | From SecLists/cirt.net archive |
| 3COM | 3COM | All | (blank) | admin | From SecLists/cirt.net archive |
| 3COM | 3COM | All | (blank) | comcomcom | From SecLists/cirt.net archive |
| 3COM | 3COM | All | <N/A> | (blank) | From SecLists/cirt.net archive |
| 3COM | 3COM | All | <N/A> | PASSWORD | From SecLists/cirt.net archive |
| 3COM | 3COM | All | <N/A> | admin | From SecLists/cirt.net archive |
| 3COM | 3COM | All | Admin | Admin | From SecLists/cirt.net archive |
| 3COM | 3COM | All | Administrator | (blank) | From SecLists/cirt.net archive |
| 3COM | 3COM | All | Administrator | admin | From SecLists/cirt.net archive |
| 3COM | 3COM | All | Type User: FORCE | (blank) | From SecLists/cirt.net archive |
| 3COM | 3COM | All | User | Password | From SecLists/cirt.net archive |
| 3COM | 3COM | All | adm | (blank) | From SecLists/cirt.net archive |
| 3COM | 3COM | All | admin | 1234admin | From SecLists/cirt.net archive |
| 3COM | 3COM | All | admin | (blank) | From SecLists/cirt.net archive |
| 3COM | 3COM | All | admin | comcomcom | From SecLists/cirt.net archive |
| 3COM | 3COM | All | admin | password | From SecLists/cirt.net archive |
| 3COM | 3COM | All | admin | synnet | From SecLists/cirt.net archive |
| 3COM | 3COM | All | adminttd | adminttd | From SecLists/cirt.net archive |
| 3COM | 3COM | All | debug | synnet | From SecLists/cirt.net archive |
| 3COM | 3COM | All | defug | synnet | From SecLists/cirt.net archive |
| 3COM | 3COM | All | manager | manager | From SecLists/cirt.net archive |
| 3COM | 3COM | All | monitor | monitor | From SecLists/cirt.net archive |
| 3COM | 3COM | All | (blank) | admin | From SecLists/cirt.net archive |
| 3COM | 3COM | All | read | synnet | From SecLists/cirt.net archive |
| 3COM | 3COM | All | recover | recover | http://support.3com.com/infodeli/tools/switches/ss3/4900/dha1770-0aaa04/htm/support/problemsolving/cliproblems.htm |
| 3COM | 3COM | All | recovery | recovery | Unit must be powered off |
| 3COM | 3COM | All | root | !root | http://support.3com.com/infodeli/tools/remote/ocradsl/20/812_cli20.pdfhttp://support.3com.com/infodeli/tools/remote/ocremote/brouters/840/2sysadmin.htm |
| 3COM | 3COM | All | security | security | From SecLists/cirt.net archive |
| 3COM | 3COM | All | tech | (blank) | From SecLists/cirt.net archive |
| 3COM | 3COM | All | tech | tech | From SecLists/cirt.net archive |
| 3COM | 3COM | All | write | synnet | From SecLists/cirt.net archive |
| Alcatel | Alcatel | All | (blank) | (blank) | http://www.speedtouch.com/support.htm |
| Alcatel | Alcatel | All | (blank) | admin | From SecLists/cirt.net archive |
| Alcatel | Alcatel | All | <N/A> | 1064 | From SecLists/cirt.net archive |
| Alcatel | Alcatel | All | SUPERUSER | ANS#150 | From SecLists/cirt.net archive |
| Alcatel Thomson | Alcatel Thomson | All | admin | admin | From SecLists/cirt.net archive |
| Alcatel | Alcatel | All | adfexc | adfexc | thanks to Nicolas Gregoire |
| Alcatel | Alcatel | All | admin | switch | From SecLists/cirt.net archive |
| Alcatel | Alcatel | All | at4400 | at4400 | thanks to Nicolas Gregoire |
| Alcatel | Alcatel | All | client | client | From SecLists/cirt.net archive |
| Alcatel | Alcatel | All | dhs3mt | dhs3mt | thanks to Nicolas Gregoire |
| Alcatel | Alcatel | All | dhs3pms | dhs3pms | thanks to Nicolas Gregoire |
| Alcatel | Alcatel | All | diag | switch | From SecLists/cirt.net archive |
| Alcatel | Alcatel | All | ftp_admi | kilo1987 | From SecLists/cirt.net archive |
| Alcatel | Alcatel | All | ftp_inst | pbxk1064 | From SecLists/cirt.net archive |
| Alcatel | Alcatel | All | ftp_nmc | tuxalize | From SecLists/cirt.net archive |
| Alcatel | Alcatel | All | ftp_oper | help1954 | From SecLists/cirt.net archive |
| Alcatel | Alcatel | All | halt | tlah | thanks to Nicolas Gregoire |
| Alcatel | Alcatel | All | install | llatsni | thanks to Nicolas Gregoire |
| Alcatel | Alcatel | All | kermit | kermit | thanks to Nicolas Gregoire |
| Alcatel | Alcatel | All | mtch | mtch | thanks to Nicolas Gregoire |
| Alcatel | Alcatel | All | mtcl | (blank) | From SecLists/cirt.net archive |
| Alcatel | Alcatel | All | mtcl | mtcl | thanks to Nicolas Gregoire |
| Alcatel | Alcatel | All | root | letacla | thanks to Nicolas Gregoire |
| Alcatel | Alcatel | All | root | permit | Perm/Config port 38036 |
| Alcatel | Alcatel | All | superuser | superuser | From SecLists/cirt.net archive |
| Allied Telesyn | Allied Telesyn | All | (blank) | manager | From SecLists/cirt.net archive |
| Allied Telesyn | Allied Telesyn | All | <N/A> | admin | From SecLists/cirt.net archive |
| Allied Telesyn | Allied Telesyn | All | admin | (blank) | From SecLists/cirt.net archive |
| Allied Telesyn | Allied Telesyn | All | manager | admin | From SecLists/cirt.net archive |
| Allied Telesyn | Allied Telesyn | All | manager | friend | From SecLists/cirt.net archive |
| Allied Telesyn | Allied Telesyn | All | manager | manager | From SecLists/cirt.net archive |
| Allied Telesyn | Allied Telesyn | All | root | (blank) | From SecLists/cirt.net archive |
| Allied Telesyn | Allied Telesyn | All | secoff | secoff | From SecLists/cirt.net archive |
| Aruba | Aruba | All | admin | admin | From SecLists/cirt.net archive |
| Aztech | Aztech | All | admin | admin | From SecLists/cirt.net archive |
| Aztech | Aztech | All | isp | isp | backdoor � not in all f/w versions |
| Aztech | Aztech | All | root | admin | From SecLists/cirt.net archive |
| Belkin | Belkin | All | (blank) | MiniAP | From SecLists/cirt.net archive |
| Belkin | Belkin | All | <N/A> | admin | From SecLists/cirt.net archive |
| Belkin | Belkin | All | admin | (blank) | From SecLists/cirt.net archive |
| Buffalo Technology | Buffalo Technology | All | admin | password | From SecLists/cirt.net archive |
| Buffalo | Buffalo | All | root | (blank) | From SecLists/cirt.net archive |
| Buffalo/MELCO | Buffalo/MELCO | All | root | (blank) | From SecLists/cirt.net archive |
| Check Point | Check Point | All | admin | admin | From SecLists/cirt.net archive |
| Check Point | Check Point | All | admin | adminadmin | From SecLists/cirt.net archive |
| Checkpoint | Checkpoint | All | admin | abc123 | From SecLists/cirt.net archive |
| Checkpoint | Checkpoint | All | admin | admin | From SecLists/cirt.net archive |
| Cisco | Cisco | All | EAdmin | (blank) | From SecLists/cirt.net archive |
| Cisco | Cisco | All | UAMIS_ | (blank) | From SecLists/cirt.net archive |
| Cisco | Cisco | All | UNITY_ | (blank) | From SecLists/cirt.net archive |
| Cisco | Cisco | All | UOMNI_ | (blank) | From SecLists/cirt.net archive |
| Cisco | Cisco | All | UVPIM_ | (blank) | From SecLists/cirt.net archive |
| Cisco | Cisco | All | (blank) | (blank) | From SecLists/cirt.net archive |
| Cisco | Cisco | All | (blank) | Cisco | From SecLists/cirt.net archive |
| Cisco | Cisco | All | (blank) | Cisco router | From SecLists/cirt.net archive |
| Cisco | Cisco | All | (blank) | _Cisco | From SecLists/cirt.net archive |
| Cisco | Cisco | All | (blank) | c | From SecLists/cirt.net archive |
| Cisco | Cisco | All | (blank) | cc | From SecLists/cirt.net archive |
| Cisco | Cisco | All | (blank) | changeit | http://160.78.48.20/vpn/software/How_to_use_Webvpn_with_Citrix_Metaframe.pdf |
| Cisco | Cisco | All | (blank) | letmein | From SecLists/cirt.net archive |
| Cisco | Cisco | All | (blank) | public/private/secret | From SecLists/cirt.net archive |
| Cisco | Cisco | All | (blank) | riverhead | http://www.cisco.com/en/US/products/ps5888/prod_release_note09186a0080237333.html |
| Cisco | Cisco | All | <N/A> | Cisco router | From SecLists/cirt.net archive |
| Cisco | Cisco | All | <N/A> | ILMI | From SecLists/cirt.net archive |
| Cisco | Cisco | All | <N/A> | c | From SecLists/cirt.net archive |
| Cisco | Cisco | All | <N/A> | cable-docsis | From SecLists/cirt.net archive |
| Cisco | Cisco | All | <N/A> | cc | From SecLists/cirt.net archive |
| Cisco | Cisco | All | <N/A> | cisco | From SecLists/cirt.net archive |
| Cisco | Cisco | All | Administrator | admin | From SecLists/cirt.net archive |
| Cisco | Cisco | All | Administrator | changeme | From SecLists/cirt.net archive |
| Cisco | Cisco | All | CISCO15 | otbu+1 | From SecLists/cirt.net archive |
| Cisco | Cisco | All | Cisco | Cisco | From SecLists/cirt.net archive |
| Cisco | Cisco | All | ESubscriber | (blank) | From SecLists/cirt.net archive |
| Cisco | Cisco | All | End User | 7936 | From SecLists/cirt.net archive |
| Cisco | Cisco | All | admin | (blank) | From SecLists/cirt.net archive |
| Cisco | Cisco | All | admin | admin | From SecLists/cirt.net archive |
| Cisco | Cisco | All | admin | changeme | From SecLists/cirt.net archive |
| Cisco | Cisco | All | admin | cisco | From SecLists/cirt.net archive |
| Cisco | Cisco | All | admin | default | From SecLists/cirt.net archive |
| Cisco | Cisco | All | admin | diamond | From SecLists/cirt.net archive |
| Cisco | Cisco | All | admin | tsunami | From SecLists/cirt.net archive |
| Cisco | Cisco | All | bbsd-client | NULL | From SecLists/cirt.net archive |
| Cisco | Cisco | All | bbsd-client | changeme2 | From SecLists/cirt.net archive |
| Cisco | Cisco | All | bubba | (unknown) | From SecLists/cirt.net archive |
| Cisco | Cisco | All | cisco | (blank) | From SecLists/cirt.net archive |
| Cisco | Cisco | All | cmaker | cmaker | From SecLists/cirt.net archive |
| Cisco | Cisco | All | enable | (blank) | From SecLists/cirt.net archive |
| Cisco | Cisco | All | enable | cisco | From SecLists/cirt.net archive |
| Cisco | Cisco | All | guest | (blank) | From SecLists/cirt.net archive |
| Cisco | Cisco | All | hsa | hsadb | From SecLists/cirt.net archive |
| Cisco | Cisco | All | netrangr | attack | From SecLists/cirt.net archive |
| Cisco | Cisco | All | pnadmin | pnadmin | From SecLists/cirt.net archive |
| Cisco | Cisco | All | praisenetwork | perfectpraise | From SecLists/cirt.net archive |
| Cisco | Cisco | All | private ReadWrite access | secret | From SecLists/cirt.net archive |
| Cisco | Cisco | All | public ReadOnly access | secret | From SecLists/cirt.net archive |
| Cisco | Cisco | All | ripeop | (blank) | From SecLists/cirt.net archive |
| Cisco | Cisco | All | root | attack | From SecLists/cirt.net archive |
| Cisco | Cisco | All | root | Cisco | From SecLists/cirt.net archive |
| Cisco | Cisco | All | root | blender | From SecLists/cirt.net archive |
| Cisco | Cisco | All | root | password | Added by DPL admin. From |
| Cisco | Cisco | All | root | secur4u | http://www.cisco.com/c/en/us/td/docs/security/physical_security/video_surveillance/network/vsm/6_3/user_guide/cvsm_6_3/overview.html#wp1035089 |
| Cisco | Cisco | All | sa | (blank) | From SecLists/cirt.net archive |
| Cisco | Cisco | All | technician | 2 + last 4 of Audio | From SecLists/cirt.net archive |
| Cisco | Cisco | All | uwmadmin | password | http://www.cisco.com/c/en/us/td/docs/cloud_services/cisco_modeling_labs/v100/installation/guide/administrator/b_cml_install_sys_admin/b_cml_install_sys_admin_chapter_0111.html |
| Cisco | Cisco | All | wlse | wlsedb | From SecLists/cirt.net archive |
| Cisco | Cisco | All | wlseuser | wlsepassword | From SecLists/cirt.net archive |
| Cisco-Arrowpoint | Cisco-Arrowpoint | All | admin | system | From SecLists/cirt.net archive |
| D-Link | D-Link | All | (blank) | admin | From SecLists/cirt.net archive |
| D-Link | D-Link | All | (blank) | private | From SecLists/cirt.net archive |
| D-Link | D-Link | All | (blank) | public | From SecLists/cirt.net archive |
| D-Link | D-Link | All | <N/A> | admin | From SecLists/cirt.net archive |
| D-Link | D-Link | All | Admin | (blank) | From SecLists/cirt.net archive |
| D-Link | D-Link | All | Alphanetworks | wrgg15_di524 | From SecLists/cirt.net archive |
| D-Link | D-Link | All | D-Link | D-Link | From SecLists/cirt.net archive |
| D-Link | D-Link | All | admin | admin | From SecLists/cirt.net archive |
| D-Link | D-Link | All | admin | gvt12345 | From SecLists/cirt.net archive |
| D-Link | D-Link | All | admin | (blank) | From SecLists/cirt.net archive |
| D-Link | D-Link | All | admin | password | hardcoded for Verizon FiOS |
| D-Link | D-Link | All | admin | public | From SecLists/cirt.net archive |
| D-Link | D-Link | All | admin | year2000 | From SecLists/cirt.net archive |
| D-Link | D-Link | All | dont need one | admin | From SecLists/cirt.net archive |
| D-Link | D-Link | All | (blank) | (blank) | From SecLists/cirt.net archive |
| D-Link | D-Link | All | (blank) | private | From SecLists/cirt.net archive |
| D-Link | D-Link | All | root | admin | From SecLists/cirt.net archive |
| D-Link | D-Link | All | user | (blank) | by rootkid |
| D-Link | D-Link | All | user | (blank) | From SecLists/cirt.net archive |
| Dlink | Dlink | All | admin | (blank) | From SecLists/cirt.net archive |
| Dlink | Dlink | All | admin | admin | From SecLists/cirt.net archive |
| Dlink | Dlink | All | admin | public | From SecLists/cirt.net archive |
| Draytek Corp | Draytek Corp | All | admin | (blank) | From SecLists/cirt.net archive |
| Draytek | Draytek | All | Draytek | 1234 | From SecLists/cirt.net archive |
| Draytek | Draytek | All | admin | (blank) | From SecLists/cirt.net archive |
| Draytek | Draytek | All | admin | admin | From SecLists/cirt.net archive |
| Edimax | Edimax | All | admin | 123 | From SecLists/cirt.net archive |
| Edimax | Edimax | All | admin | 1234 | From SecLists/cirt.net archive |
| Edimax | Edimax | All | admin | (blank) | From SecLists/cirt.net archive |
| Edimax | Edimax | All | admin | epicrouter | From SecLists/cirt.net archive |
| Edimax | Edimax | All | admin | password | From SecLists/cirt.net archive |
| Edimax | Edimax | All | admin | su@psir | From SecLists/cirt.net archive |
| Edimax | Edimax | All | edimax | software01 | for most Edimax HW???? |
| Edimax | Edimax | All | guest | 1234 | From SecLists/cirt.net archive |
| Edimax | Edimax | All | guest | (blank) | From SecLists/cirt.net archive |
| Extreme Networks | Extreme Networks | All | admin | (blank) | From SecLists/cirt.net archive |
| Fortigate | Fortigate | All | admin | (blank) | From SecLists/cirt.net archive |
| Fortinet | Fortinet | All | (blank) | bcpb(serial number of the firewall) | From SecLists/cirt.net archive |
| Fortinet | Fortinet | All | admin | (blank) | From SecLists/cirt.net archive |
| Fortinet | Fortinet | All | maintainer | admin | From SecLists/cirt.net archive |
| Fortinet | Fortinet | All | maintainer | bcpb[SERIAL NO.] | From SecLists/cirt.net archive |
| Fortinet | Fortinet | All | maintainer | pbcpbn(add-serial-number) | From SecLists/cirt.net archive |
| Huawei | Huawei | All | TMAR#HWMT8007079 | (blank) | From SecLists/cirt.net archive |
| Huawei Technologies Co | Huawei Technologies Co | All | TMAR#HWMT8007079 | (blank) | From SecLists/cirt.net archive |
| Huawei Technologies Co | Huawei Technologies Co | All | admin | admin | From SecLists/cirt.net archive |
| Huawei | Huawei | All | admin | admin | From SecLists/cirt.net archive |
| Huawei | Huawei | All | root | Changeme_123 | https://forum.huawei.com/enterprise/en/default-ips-usernames-and-passwords-of-huawei-transmission-products/thread/551181-875 |
| Huawei | Huawei | All | (blank) | Changeme123 | https://support.huawei.com/enterprise/en/doc/EDOC1000118783?section=j004 |
| Juniper | Juniper | All | admin | abc123 | https://kb.juniper.net/InfoCenter/index?page=content&id=KB26220&actp=search |
| Juniper | Juniper | All | admin | netscreen | From SecLists/cirt.net archive |
| Juniper | Juniper | All | admin | peribit | From SecLists/cirt.net archive |
| Juniper | Juniper | All | netscreen | netscreen | From SecLists/cirt.net archive |
| Juniper | Juniper | All | redline | redline | From SecLists/cirt.net archive |
| Juniper | Juniper | All | serial# | serial# | Resets to factory settings |
| Juniper | Juniper | All | super | juniper123 | https://kb.juniper.net/InfoCenter/index?page=content&id=KB26220&actp=search |
| Linksys | Linksys | All | (blank) | admin | From SecLists/cirt.net archive |
| Linksys | Linksys | All | (blank) | epicrouter | From SecLists/cirt.net archive |
| Linksys | Linksys | All | <N/A> | (blank) | From SecLists/cirt.net archive |
| Linksys | Linksys | All | <N/A> | admin | From SecLists/cirt.net archive |
| Linksys | Linksys | All | Administrator | admin | From SecLists/cirt.net archive |
| Linksys | Linksys | All | admin | (blank) | From SecLists/cirt.net archive |
| Linksys | Linksys | All | admin | admin | From SecLists/cirt.net archive |
| Linksys | Linksys | All | comcast | 1234 | From SecLists/cirt.net archive |
| Linksys | Linksys | All | root | orion99 | From SecLists/cirt.net archive |
| Linksys | Linksys | All | user | tivonpw | From SecLists/cirt.net archive |
| MikroTik | MikroTik | All | admin | (blank) | From SecLists/cirt.net archive |
| Netgear | Netgear | All | (blank) | 1234 | From SecLists/cirt.net archive |
| Netgear | Netgear | All | (blank) | admin | From SecLists/cirt.net archive |
| Netgear | Netgear | All | (blank) | private | From SecLists/cirt.net archive |
| Netgear | Netgear | All | (blank) | zebra | From SecLists/cirt.net archive |
| Netgear | Netgear | All | <N/A> | (blank) | From SecLists/cirt.net archive |
| Netgear | Netgear | All | <N/A> | admin | From SecLists/cirt.net archive |
| Netgear | Netgear | All | <N/A> | password | From SecLists/cirt.net archive |
| Netgear | Netgear | All | Admin | password | From SecLists/cirt.net archive |
| Netgear | Netgear | All | Gearguy | Geardog | From SecLists/cirt.net archive |
| Netgear | Netgear | All | admin | 1234 | From SecLists/cirt.net archive |
| Netgear | Netgear | All | admin | (blank) | From SecLists/cirt.net archive |
| Netgear | Netgear | All | admin | admin | From SecLists/cirt.net archive |
| Netgear | Netgear | All | admin | draadloos | From SecLists/cirt.net archive |
| Netgear | Netgear | All | admin | infrant1 | Upto v3 firmware |
| Netgear | Netgear | All | admin | netgear1 | v4 firmware onwards |
| Netgear | Netgear | All | admin | setup | From SecLists/cirt.net archive |
| Netgear | Netgear | All | comcast | 1234 | From SecLists/cirt.net archive |
| Netgear | Netgear | All | cusadmin | highspeed | From SecLists/cirt.net archive |
| Netgear | Netgear | All | super | 5777364 | From SecLists/cirt.net archive |
| Netgear | Netgear | All | superman | 21241036 | From SecLists/cirt.net archive |
| Netscreen | Netscreen | All | <N/A> | (blank) | From SecLists/cirt.net archive |
| Netscreen | Netscreen | All | Administrator | (blank) | From SecLists/cirt.net archive |
| Netscreen | Netscreen | All | admin | (blank) | From SecLists/cirt.net archive |
| Netscreen | Netscreen | All | admin | netscreen | From SecLists/cirt.net archive |
| Netscreen | Netscreen | All | netscreen | netscreen | From SecLists/cirt.net archive |
| Netscreen | Netscreen | All | operator | (blank) | From SecLists/cirt.net archive |
| Nortel | Nortel | All | 266344 | 266344 | From SecLists/cirt.net archive |
| Nortel | Nortel | All | (blank) | 0 | From SecLists/cirt.net archive |
| Nortel | Nortel | All | (blank) | (blank) | From SecLists/cirt.net archive |
| Nortel | Nortel | All | (blank) | l1 | From SecLists/cirt.net archive |
| Nortel | Nortel | All | (blank) | l2 | From SecLists/cirt.net archive |
| Nortel | Nortel | All | (blank) | ro | From SecLists/cirt.net archive |
| Nortel | Nortel | All | (blank) | rw | From SecLists/cirt.net archive |
| Nortel | Nortel | All | (blank) | rwa | From SecLists/cirt.net archive |
| Nortel | Nortel | All | (blank) | secure | From SecLists/cirt.net archive |
| Nortel | Nortel | All | <N/A> | 266344 | From SecLists/cirt.net archive |
| Nortel | Nortel | All | <N/A> | (blank) | From SecLists/cirt.net archive |
| Nortel | Nortel | All | <N/A> | secure | From SecLists/cirt.net archive |
| Nortel | Nortel | All | Manager | (blank) | From SecLists/cirt.net archive |
| Nortel | Nortel | All | admin | 000000 | http://support.avaya.com/css/P8/documents/100097575 |
| Nortel | Nortel | All | admin | (blank) | http://support.avaya.com/css/P8/documents/100097575 |
| Nortel | Nortel | All | admin | admin | From SecLists/cirt.net archive |
| Nortel | Nortel | All | admin | admin000 | From SecLists/cirt.net archive |
| Nortel | Nortel | All | admin | root | From SecLists/cirt.net archive |
| Nortel | Nortel | All | admin | setup | From SecLists/cirt.net archive |
| Nortel | Nortel | All | administrator | PlsChgMe! | From SecLists/cirt.net archive |
| Nortel | Nortel | All | ccrusr | ccrusr | From SecLists/cirt.net archive |
| Nortel | Nortel | All | conferencing | admin | http://support.avaya.com/css/P8/documents/100097575 |
| Nortel | Nortel | All | debug | gubed | http://support.avaya.com/css/P8/documents/100097575 |
| Nortel | Nortel | All | distrib | distrib0 | From SecLists/cirt.net archive |
| Nortel | Nortel | All | disttech | 4tas | From SecLists/cirt.net archive |
| Nortel | Nortel | All | disttech | disttech | From SecLists/cirt.net archive |
| Nortel | Nortel | All | disttech | etas | From SecLists/cirt.net archive |
| Nortel | Nortel | All | l2 | l2 | From SecLists/cirt.net archive |
| Nortel | Nortel | All | l3 | l3 | From SecLists/cirt.net archive |
| Nortel | Nortel | All | login | 0 | AUTH codes in LD 8 |
| Nortel | Nortel | All | login | 0000 | From SecLists/cirt.net archive |
| Nortel | Nortel | All | login | 1111 | AUTH codes in LD 8 |
| Nortel | Nortel | All | login | 8429 | AUTH codes in LD 8 |
| Nortel | Nortel | All | maint | maint | From SecLists/cirt.net archive |
| Nortel | Nortel | All | maint | ntacdmax | From SecLists/cirt.net archive |
| Nortel | Nortel | All | mlusr | mlusr | From SecLists/cirt.net archive |
| Nortel | Nortel | All | ro | ro | From SecLists/cirt.net archive |
| Nortel | Nortel | All | root | 3ep5w2u | From SecLists/cirt.net archive |
| Nortel | Nortel | All | rw | rw | From SecLists/cirt.net archive |
| Nortel | Nortel | All | rwa | rwa | From SecLists/cirt.net archive |
| Nortel | Nortel | All | service | smile | From SecLists/cirt.net archive |
| Nortel | Nortel | All | spcl | 0 | AUTH codes in LD 8 |
| Nortel | Nortel | All | spcl | 0000 | From SecLists/cirt.net archive |
| Nortel | Nortel | All | supervisor | PlsChgMe! | From SecLists/cirt.net archive |
| Nortel | Nortel | All | supervisor | visor | From SecLists/cirt.net archive |
| Nortel | Nortel | All | sysadmin | nortel | From SecLists/cirt.net archive |
| Nortel | Nortel | All | system | adminpwd | From SecLists/cirt.net archive |
| Nortel | Nortel | All | tasman | tasmannet | From SecLists/cirt.net archive |
| Nortel | Nortel | All | trmcnfg | trmcnfg | From SecLists/cirt.net archive |
| Nortel | Nortel | All | user | (blank) | From SecLists/cirt.net archive |
| Nortel | Nortel | All | user | user | From SecLists/cirt.net archive |
| Nortel | Nortel | All | user | user0000 | From SecLists/cirt.net archive |
| SonicWALL | SonicWALL | All | admin | password | From SecLists/cirt.net archive |
| TrendNET | TrendNET | All | admin | password | From SecLists/cirt.net archive |
| WatchGuard | WatchGuard | All | (blank) | wg | From SecLists/cirt.net archive |
| WatchGuard | WatchGuard | All | admin | admin | http://www.watchguard.com/help/docs/v70FireboxXEdge_QS.pdf |
| WatchGuard | WatchGuard | All | admin | readwrite | http://www.watchguard.com/help/docs/wsm/xtm_11/en-us/content/en-us/basicadmin/factory_default_about_c.html |
| WatchGuard | WatchGuard | All | status | readonly | http://www.watchguard.com/help/docs/wsm/xtm_11/en-us/content/en-us/basicadmin/factory_default_about_c.html |
| Watchguard | Watchguard | All | admin | (blank) | From SecLists/cirt.net archive |
| Watchguard | Watchguard | All | user | pass | works only from the inside LAN |
| ZTE | ZTE | All | ADSL | expert03 | Default Password if user does |
| Zyxel | Zyxel | All | 1234 | 1234 | From SecLists/cirt.net archive |
| Zyxel | Zyxel | All | 192.168.1.1 60020 | @dsl_xilno | From SecLists/cirt.net archive |
| Zyxel | Zyxel | All | (blank) | 1234 | From SecLists/cirt.net archive |
| Zyxel | Zyxel | All | <N/A> | 1234 | From SecLists/cirt.net archive |
| Zyxel | Zyxel | All | <N/A> | (blank) | From SecLists/cirt.net archive |
| Zyxel | Zyxel | All | <N/A> | admin | From SecLists/cirt.net archive |
| Zyxel | Zyxel | All | Admin | atc456 | From SecLists/cirt.net archive |
| Zyxel | Zyxel | All | admin | 0000 | Password is 4 zeros. Gray router |
| Zyxel | Zyxel | All | admin | 1234 | From SecLists/cirt.net archive |
| Zyxel | Zyxel | All | admin | (blank) | terra |
| Zyxel | Zyxel | All | admin | admin | From SecLists/cirt.net archive |
| Zyxel | Zyxel | All | root | 1234 | From SecLists/cirt.net archive |
| Zyxel | Zyxel | All | webadmin | 1234 | From SecLists/cirt.net archive |
| 3COM (ssh) | 3COM (ssh) | All | admin | admin | From SecLists/cirt.net archive |
| Alcatel | Alcatel | All | (blank) | 1064 | From SecLists/cirt.net archive |
| Alcatel | Alcatel | All | (blank) | 151515 | From SecLists/cirt.net archive |
| Allied Telesyn | Allied Telesyn | All | (blank) | admin | From SecLists/cirt.net archive |
| Aruba Controller | Aruba Controller | All | admin | admin | From SecLists/cirt.net archive |
| Aruba (web) | Aruba (web) | All | admin | admin | From SecLists/cirt.net archive |
| ASUS Router | ASUS Router | All | admin | admin | From SecLists/cirt.net archive |
| Belkin | Belkin | All | admin | (blank) | From SecLists/cirt.net archive |
| Belkin | Belkin | All | (blank) | admin | From SecLists/cirt.net archive |
| Check Point 1470 appliance | Check Point 1470 appliance | All | admin | Admin123 | From SecLists/cirt.net archive |
| Checkpoint (web) | Checkpoint (web) | All | admin | abc123 | From SecLists/cirt.net archive |
| Checkpoint (web) | Checkpoint (web) | All | admin | admin | From SecLists/cirt.net archive |
| Cisco | Cisco | All | admin | localadmin | From SecLists/cirt.net archive |
| Cisco Aironet (ssh) | Cisco Aironet (ssh) | All | Cisco | Cisco | From SecLists/cirt.net archive |
| Cisco | Cisco | All | bbsd-client | (blank) | From SecLists/cirt.net archive |
| Cisco | Cisco | All | (blank) | cable-docsis | From SecLists/cirt.net archive |
| Cisco | Cisco | All | (blank) | ILMI | From SecLists/cirt.net archive |
| Cisco Collaboration Endpoint (general) | Cisco Collaboration Endpoint (general) | All | cisco | admin | From SecLists/cirt.net archive |
| Cisco Guard (snmp) | Cisco Guard (snmp) | All | (blank) | riverhead | From SecLists/cirt.net archive |
| Cisco (IPMI) | Cisco (IPMI) | All | admin | password | From SecLists/cirt.net archive |
| Cisco | Cisco | All | scpuser | scpuser | From SecLists/cirt.net archive |
| Cisco (ssh) | Cisco (ssh) | All | cisco | cisco | From SecLists/cirt.net archive |
| Cisco (ssh) | Cisco (ssh) | All | pix | cisco | From SecLists/cirt.net archive |
| Cisco Systems (general) | Cisco Systems (general) | All | cisco | cisco | From SecLists/cirt.net archive |
| D-Link | D-Link | All | (blank) | (blank) | From SecLists/cirt.net archive |
| D-Link DIR300 (CVE-2024-41616) | D-Link DIR300 (CVE-2024-41616) | All | Alphanetworks | wrgg19_c_dlwbr_dir300 | From SecLists/cirt.net archive |
| D-Link DIR845L | D-Link DIR845L | All | Alphanetworks | wrgnd21_dlob.hans_dir845 | From SecLists/cirt.net archive |
| D-Link Router | D-Link Router | All | admin | admin | From SecLists/cirt.net archive |
| D-Link Router | D-Link Router | All | admin | (blank) | From SecLists/cirt.net archive |
| Dlink (web) | Dlink (web) | All | 1234 | 1234 | From SecLists/cirt.net archive |
| Dlink (web) | Dlink (web) | All | admin | admin | From SecLists/cirt.net archive |
| Dlink (web) | Dlink (web) | All | root | 12345 | From SecLists/cirt.net archive |
| Dlink (web) | Dlink (web) | All | root | root | From SecLists/cirt.net archive |
| Fortinet FortiManager | Fortinet FortiManager | All | admin | (blank) | From SecLists/cirt.net archive |
| fortinet (web) | fortinet (web) | All | admin | (blank) | From SecLists/cirt.net archive |
| fortinet (web) | fortinet (web) | All | maintainer | admin | From SecLists/cirt.net archive |
| fortinet (web) | fortinet (web) | All | maintainer | bcpb+serial# | From SecLists/cirt.net archive |
| Huawei EG8245H | Huawei EG8245H | All | Epuser | userEp | From SecLists/cirt.net archive |
| Huawei HG8245 | Huawei HG8245 | All | telecomadmin | admintelecom | From SecLists/cirt.net archive |
| Huawei S2700 | Huawei S2700 | All | admin | admin@huawei.com | From SecLists/cirt.net archive |
| Huawei S3700 | Huawei S3700 | All | admin | admin@huawei.com | From SecLists/cirt.net archive |
| Huawei S5700 | Huawei S5700 | All | admin | admin@huawei.com | From SecLists/cirt.net archive |
| Huawei S6700 | Huawei S6700 | All | admin | admin@huawei.com | From SecLists/cirt.net archive |
| huawei (ssh) | huawei (ssh) | All | admin | admin | From SecLists/cirt.net archive |
| huawei (ssh) | huawei (ssh) | All | admin | (blank) | From SecLists/cirt.net archive |
| huawei (ssh) | huawei (ssh) | All | digicel | digicel | From SecLists/cirt.net archive |
| huawei (ssh) | huawei (ssh) | All | telecomadmin | admintelecom | From SecLists/cirt.net archive |
| huawei (ssh) | huawei (ssh) | All | user | HuaweiUser | From SecLists/cirt.net archive |
| huawei (ssh) | huawei (ssh) | All | user | user | From SecLists/cirt.net archive |
| huawei (ssh) | huawei (ssh) | All | vodafone | vodafone | From SecLists/cirt.net archive |
| IBM Storwize V7000 Unified (ssh) | IBM Storwize V7000 Unified (ssh) | All | admin | admin0001 | From SecLists/cirt.net archive |
| IBM Storwize V7000 Unified (ssh) | IBM Storwize V7000 Unified (ssh) | All | root | Passw0rd | From SecLists/cirt.net archive |
| IBM Storwize V7000 Unified (ssh) | IBM Storwize V7000 Unified (ssh) | All | superuser | passw0rd | From SecLists/cirt.net archive |
| Juniper ScreenOS/Netscreen (telnet) | Juniper ScreenOS/Netscreen (telnet) | All | netscreen | <<< %s(un='%s') = %u | From SecLists/cirt.net archive |
| juniper (ssh) | juniper (ssh) | All | admin | abc123 | From SecLists/cirt.net archive |
| Juniper (ssh) | Juniper (ssh) | All | admin | netscreen | From SecLists/cirt.net archive |
| Juniper (ssh) | Juniper (ssh) | All | admin | peribit | From SecLists/cirt.net archive |
| juniper (ssh) | juniper (ssh) | All | admin | <<< %s(un=\'%s\') = %u. | From SecLists/cirt.net archive |
| Juniper (ssh) | Juniper (ssh) | All | netscreen | netscreen | From SecLists/cirt.net archive |
| Juniper (ssh) | Juniper (ssh) | All | redline | redline | From SecLists/cirt.net archive |
| Juniper (ssh) | Juniper (ssh) | All | serial# | serial# | From SecLists/cirt.net archive |
| juniper (ssh) | juniper (ssh) | All | super | juniper123 | From SecLists/cirt.net archive |
| Linksys | Linksys | All | (blank) | (blank) | From SecLists/cirt.net archive |
| Linksys Router | Linksys Router | All | admin | admin | From SecLists/cirt.net archive |
| linksys (ssh) | linksys (ssh) | All | admin | admin | From SecLists/cirt.net archive |
| linksys (ssh) | linksys (ssh) | All | admin | password | From SecLists/cirt.net archive |
| linksys (ssh) | linksys (ssh) | All | linksys | (blank) | From SecLists/cirt.net archive |
| linksys (ssh) | linksys (ssh) | All | root | admin | From SecLists/cirt.net archive |
| MikroTik RouterOS | MikroTik RouterOS | All | admin | (blank) | From SecLists/cirt.net archive |
| Netgear | Netgear | All | (blank) | (blank) | From SecLists/cirt.net archive |
| Netgear | Netgear | All | (blank) | password | From SecLists/cirt.net archive |
| Netgear Router | Netgear Router | All | admin | password | From SecLists/cirt.net archive |
| Netscreen | Netscreen | All | (blank) | (blank) | From SecLists/cirt.net archive |
| Nortel | Nortel | All | (blank) | 266344 | From SecLists/cirt.net archive |
| Nortel Integrated Call Director (web) | Nortel Integrated Call Director (web) | All | admin | admin | From SecLists/cirt.net archive |
| Palo Alto GlobalProtect Gateway | Palo Alto GlobalProtect Gateway | All | admin | admin | From SecLists/cirt.net archive |
| Sophos UTM (web) | Sophos UTM (web) | All | admin | admin | From SecLists/cirt.net archive |
| TP-Link | TP-Link | All | admin | admin | From SecLists/cirt.net archive |
| TP-Link Router | TP-Link Router | All | admin | admin | From SecLists/cirt.net archive |
| Ubiquiti EdgeOS (web) | Ubiquiti EdgeOS (web) | All | ubnt | ubnt | From SecLists/cirt.net archive |
| Ubiquiti EdgeRouter | Ubiquiti EdgeRouter | All | ubnt | ubnt | From SecLists/cirt.net archive |
| ubiquiti (ssh) | ubiquiti (ssh) | All | admin | admin | From SecLists/cirt.net archive |
| ubiquiti (ssh) | ubiquiti (ssh) | All | root | ubnt | From SecLists/cirt.net archive |
| ubiquiti (ssh) | ubiquiti (ssh) | All | ubnt | ubnt | From SecLists/cirt.net archive |
| Ubiquiti UniFi (web) | Ubiquiti UniFi (web) | All | ubnt | ubnt | From SecLists/cirt.net archive |
| Unifi | Unifi | All | root | ubnt | From SecLists/cirt.net archive |
| Unifi | Unifi | All | root | ui | From SecLists/cirt.net archive |
| Unifi | Unifi | All | ubnt | ubnt | From SecLists/cirt.net archive |
| Unifi | Unifi | All | ui | ui | From SecLists/cirt.net archive |
| zte (ssh) | zte (ssh) | All | admin | admin | From SecLists/cirt.net archive |
| zte (ssh) | zte (ssh) | All | on | on | From SecLists/cirt.net archive |
| zte (ssh) | zte (ssh) | All | root | W!n0&oO7. | From SecLists/cirt.net archive |
| zte (ssh) | zte (ssh) | All | root | Zte521 | From SecLists/cirt.net archive |
| zte (ssh) | zte (ssh) | All | user | user | From SecLists/cirt.net archive |
| zte (ssh) | zte (ssh) | All | ZXDSL | ZXDSL | From SecLists/cirt.net archive |
| Zyxel | Zyxel | All | (blank) | admin | From SecLists/cirt.net archive |
| Zyxel | Zyxel | All | (blank) | (blank) | From SecLists/cirt.net archive |
| Zyxel NWA/NAP/WAC wireless access point series (ftp) | Zyxel NWA/NAP/WAC wireless access point series (ftp) | All | devicehaecived | 1234 | From SecLists/cirt.net archive |
| ZyXEL Router | ZyXEL Router | All | admin | 1234 | From SecLists/cirt.net archive |
| Zyxel (ssh) | Zyxel (ssh) | All | zyfwp | PrOw!aN_fXp | From SecLists/cirt.net archive |

## 4. OOB / hardware management

| Product | Vendor | Version(s) | Username | Password | Notes |
|---|---|---|---|---|---|
| Avocent KVM | Avocent | All | Admin | (blank) | Web admin |
| Raritan Dominion KX | Raritan | All | admin | raritan | Web/SSH |
| Intel AMT | Intel | All | admin | admin | MEBx; must change on enable |
| iRMC S4/S5 | Fujitsu | All | admin | admin | Web/IPMI |
| UCS Manager | Cisco | All | admin | (set on install) | Web admin |
| CIMC | Cisco | All | admin | password | UCS C-series web/IPMI |
| IPMI BMC | Supermicro | Newer | ADMIN | (unique per board) | Printed on label |
| XCC (XClarity Controller) | Lenovo | All | USERID | PASSW0RD | IPMI/web; must change on first login (newer) |
| Integrated Management Module (IMM) | IBM/Lenovo | All | USERID | PASSW0RD | IPMI/web; zero is digit zero |
| iLO 4/5 | HP/HPE | All | admin | admin | Some early units |
| iLO 2/3/4 | HP/HPE | All | Administrator | (unique 8-char) | Printed on tag |
| iDRAC 9 | Dell | >=9 | root | (unique per service tag) | Printed on label; must change on first login |
| iDRAC 6/7/8 | Dell | All | root | calvin | Web/IPMI/SSH; kept default unless changed |
| SuperMicro | SuperMicro | All | (blank) | ksdjfg934t | From SecLists/cirt.net archive |
| SuperMicro | SuperMicro | All | <N/A> | ksdjfg934t | From SecLists/cirt.net archive |
| Supermicro | Supermicro | All | ADMIN | admin | From SecLists/cirt.net archive |
| Asus iKVM BMC (IPMI) | Asus iKVM BMC (IPMI) | All | admin | admin | From SecLists/cirt.net archive |
| avigilon (web) | avigilon (web) | All | admin | admin | From SecLists/cirt.net archive |
| avigilon (web) | avigilon (web) | All | Administrator | (blank) | From SecLists/cirt.net archive |
| Dell iDRAC (IPMI) | Dell iDRAC (IPMI) | All | root | calvin | From SecLists/cirt.net archive |
| Dell iDRAC (web) | Dell iDRAC (web) | All | root | calvin | From SecLists/cirt.net archive |
| Fujitsu iRMC (IPMI) | Fujitsu iRMC (IPMI) | All | admin | admin | From SecLists/cirt.net archive |
| IBM IMM (IPMI) | IBM IMM (IPMI) | All | USERID | PASSW0RD | From SecLists/cirt.net archive |
| IBM IMM (web) | IBM IMM (web) | All | USERID | PASSW0RD | From SecLists/cirt.net archive |
| iDRAC (Dell) | iDRAC (Dell) | All | root | calvin | From SecLists/cirt.net archive |
| Oracle ILOM/Sun ILOM (IPMI) | Oracle ILOM/Sun ILOM (IPMI) | All | root | changeme | From SecLists/cirt.net archive |
| Supermicro IPMI | Supermicro IPMI | All | ADMIN | ADMIN | From SecLists/cirt.net archive |
| Supermicro SIM (IPMI) | Supermicro SIM (IPMI) | All | ADMIN | ADMIN | From SecLists/cirt.net archive |
| Supermicro (web) | Supermicro (web) | All | ADMIN | ADMIN | From SecLists/cirt.net archive |

## 5. Hypervisors & virt mgmt

| Product | Vendor | Version(s) | Username | Password | Notes |
|---|---|---|---|---|---|
| Nutanix AHV host | Nutanix | All | root | nutanix/4u | SSH |
| Nutanix CVM | Nutanix | All | nutanix | nutanix/4u | SSH |
| Nutanix Prism | Nutanix | All | admin | Nutanix/4u | Web admin; must change on first login |
| XenServer | Citrix | All | root | (set on install) | XenCenter/SSH |
| oVirt Engine | oVirt | All | admin@internal | (set on install) | Web admin |
| Proxmox VE | Proxmox | All | root | (set on install) | Web/SSH; PAM auth |
| vRealize Operations | VMware | All | admin | (set on install) | Web admin |
| vCenter Server Appliance | VMware | All | administrator@vsphere.local | (set on install) | Web admin |
| ESXi | VMware | All | root | (set on install) | Web/SSH; password set during install |
| Nutanix | Nutanix | All | nutanix | 4u | From SecLists/cirt.net archive |
| Proxmox VE (web) | Proxmox VE (web) | All | root | proxmox | From SecLists/cirt.net archive |
| VMware ESXi (web) | VMware ESXi (web) | All | root | vmware | From SecLists/cirt.net archive |

## 6. Databases

| Product | Vendor | Version(s) | Username | Password | Notes |
|---|---|---|---|---|---|
| Informix | IBM | All | informix | informix | Common dev default |
| SAP HANA | SAP | All | SYSTEM | (set on install) | Master password during install |
| Sybase ASE | Sybase | All | sso | (blank) | TDS |
| Sybase ASE | Sybase | All | sa | (blank) | TDS |
| DB2 admin | IBM | All | db2admin | db2admin | Windows install default |
| DB2 instance | IBM | All | db2inst1 | db2inst1 | Common install default |
| InfluxDB | InfluxData | >=2 | (set on install) | (set on install) | Setup wizard |
| InfluxDB | InfluxData | <2 | (blank) | (blank) | No auth by default |
| Cassandra | Apache | All | cassandra | cassandra | CQL |
| CouchDB | CouchDB | >=3.x | admin | (set on install) | Must set |
| CouchDB | CouchDB | <3.x | (blank) | (blank) | Admin Party mode |
| Couchbase | Couchbase | All | Administrator | password | Web admin (must set) |
| Memcached | Memcached | All | (blank) | (blank) | No auth |
| Kibana | Elastic | >=8 | elastic | (from elasticsearch) | Web admin |
| Elasticsearch | Elastic | >=8 | elastic | (generated on first start) | Auto-configured TLS+auth |
| Elasticsearch | Elastic | <8 | (blank) | (blank) | No auth by default; X-Pack required |
| Redis | Redis | <6 | (blank) | (blank) | No auth by default |
| Mongo Express | Mongo Express | All | admin | pass | Web admin |
| MongoDB | MongoDB | <3.6 | (blank) | (blank) | No auth by default; bound to localhost in newer |
| PostgreSQL | PostgreSQL | All | postgres | postgres | Common dev default; varies by distro/installer |
| MariaDB root | MariaDB | All | root | (blank or socket) | Socket auth by default on Linux |
| MySQL root | MySQL | >=5.7 | root | (unique generated) | Logged to error log on install |
| MySQL root | MySQL | <5.7 | root | (blank) | TCP/socket; newer require socket auth |
| MS SQL Server (legacy) | Microsoft | <2005 | sa | (blank) | Default for SQL2000 mixed-mode |
| MS SQL Server sa | Microsoft | All | sa | (set on install) | TDS; mixed-mode auth |
| Oracle XE 11g | Oracle | 11g XE | SYS | oracle | SQL*Net |
| Firebird Project | Firebird Project | All | SYSDBA | masterkey | From SecLists/cirt.net archive |
| Firebird | Firebird | All | SYSDBA | masterkey | From SecLists/cirt.net archive |
| Informix | Informix | All | informix | informix | From SecLists/cirt.net archive |
| MySQL | MySQL | All | admin@example.com | admin | From SecLists/cirt.net archive |
| MySQL | MySQL | All | root | (blank) | From SecLists/cirt.net archive |
| MySQL | MySQL | All | superdba | admin | From SecLists/cirt.net archive |
| Oracle | Oracle | All | <N/A> | (blank) | From SecLists/cirt.net archive |
| Oracle | Oracle | All | ADAMS | WOOD | From SecLists/cirt.net archive |
| Oracle | Oracle | All | ADLDEMO | ADLDEMO | From SecLists/cirt.net archive |
| Oracle | Oracle | All | ADMIN | JETSPEED | From SecLists/cirt.net archive |
| Oracle | Oracle | All | ADMIN | WELCOME | From SecLists/cirt.net archive |
| Oracle | Oracle | All | ADMINISTRATOR | ADMINISTRATOR | From SecLists/cirt.net archive |
| Oracle | Oracle | All | ADMINISTRATOR | admin | From SecLists/cirt.net archive |
| Oracle | Oracle | All | ANDY | SWORDFISH | From SecLists/cirt.net archive |
| Oracle | Oracle | All | AP | AP | From SecLists/cirt.net archive |
| Oracle | Oracle | All | APPLSYS | APPLSYS | From SecLists/cirt.net archive |
| Oracle | Oracle | All | APPLSYS | FND | From SecLists/cirt.net archive |
| Oracle | Oracle | All | APPLSYSPUB | FNDPUB | From SecLists/cirt.net archive |
| Oracle | Oracle | All | APPS | APPS | From SecLists/cirt.net archive |
| Oracle | Oracle | All | APPUSER | APPUSER | From SecLists/cirt.net archive |
| Oracle | Oracle | All | AQ | AQ | From SecLists/cirt.net archive |
| Oracle | Oracle | All | AQDEMO | AQDEMO | From SecLists/cirt.net archive |
| Oracle | Oracle | All | AQJAVA | AQJAVA | From SecLists/cirt.net archive |
| Oracle | Oracle | All | AQUSER | AQUSER | From SecLists/cirt.net archive |
| Oracle | Oracle | All | AUDIOUSER | AUDIOUSER | From SecLists/cirt.net archive |
| Oracle | Oracle | All | AURORA$JIS$UTILITY$ | (blank) | From SecLists/cirt.net archive |
| Oracle | Oracle | All | AURORA$ORB$UNAUTHENTICATED | INVALID | From SecLists/cirt.net archive |
| Oracle | Oracle | All | AURORA@ORB@UNAUTHENTICATED | INVALID | From SecLists/cirt.net archive |
| Oracle | Oracle | All | BC4J | BC4J | From SecLists/cirt.net archive |
| Oracle | Oracle | All | BLAKE | PAPER | From SecLists/cirt.net archive |
| Oracle | Oracle | All | BRIO_ADMIN | BRIO_ADMIN | From SecLists/cirt.net archive |
| Oracle | Oracle | All | CATALOG | CATALOG | From SecLists/cirt.net archive |
| Oracle | Oracle | All | CDEMO82 | CDEMO82 | From SecLists/cirt.net archive |
| Oracle | Oracle | All | CDEMOCOR | CDEMOCOR | From SecLists/cirt.net archive |
| Oracle | Oracle | All | CDEMORID | CDEMORID | From SecLists/cirt.net archive |
| Oracle | Oracle | All | CDEMOUCB | CDEMOUCB | From SecLists/cirt.net archive |
| Oracle | Oracle | All | CENTRA | CENTRA | From SecLists/cirt.net archive |
| Oracle | Oracle | All | CIDS | CIDS | From SecLists/cirt.net archive |
| Oracle | Oracle | All | CIS | CIS | From SecLists/cirt.net archive |
| Oracle | Oracle | All | CISINFO | CISINFO | From SecLists/cirt.net archive |
| Oracle | Oracle | All | CLARK | CLOTH | From SecLists/cirt.net archive |
| Oracle | Oracle | All | COMPANY | COMPANY | From SecLists/cirt.net archive |
| Oracle | Oracle | All | COMPIERE | COMPIERE | From SecLists/cirt.net archive |
| Oracle | Oracle | All | CQSCHEMAUSER | PASSWORD | From SecLists/cirt.net archive |
| Oracle | Oracle | All | CSMIG | CSMIG | From SecLists/cirt.net archive |
| Oracle | Oracle | All | CTXDEMO | CTXDEMO | From SecLists/cirt.net archive |
| Oracle | Oracle | All | CTXSYS | (blank) | From SecLists/cirt.net archive |
| Oracle | Oracle | All | CTXSYS | CTXSYS | From SecLists/cirt.net archive |
| Oracle | Oracle | All | DBI | MUMBLEFRATZ | From SecLists/cirt.net archive |
| Oracle | Oracle | All | DBSNMP | DBSNMP | From SecLists/cirt.net archive |
| Oracle | Oracle | All | DEMO | DEMO | From SecLists/cirt.net archive |
| Oracle | Oracle | All | DEMO8 | DEMO8 | From SecLists/cirt.net archive |
| Oracle | Oracle | All | DEMO9 | DEMO9 | From SecLists/cirt.net archive |
| Oracle | Oracle | All | DES | DES | From SecLists/cirt.net archive |
| Oracle | Oracle | All | DEV2000_DEMOS | DEV2000_DEMOS | From SecLists/cirt.net archive |
| Oracle | Oracle | All | DIP | DIP | From SecLists/cirt.net archive |
| Oracle | Oracle | All | DISCOVERER_ADMIN | DISCOVERER_ADMIN | From SecLists/cirt.net archive |
| Oracle | Oracle | All | DSGATEWAY | DSGATEWAY | From SecLists/cirt.net archive |
| Oracle | Oracle | All | DSSYS | DSSYS | From SecLists/cirt.net archive |
| Oracle | Oracle | All | EJSADMIN | EJSADMIN | From SecLists/cirt.net archive |
| Oracle | Oracle | All | EMP | EMP | From SecLists/cirt.net archive |
| Oracle | Oracle | All | ESTOREUSER | ESTORE | From SecLists/cirt.net archive |
| Oracle | Oracle | All | EVENT | EVENT | From SecLists/cirt.net archive |
| Oracle | Oracle | All | EXFSYS | EXFSYS | From SecLists/cirt.net archive |
| Oracle | Oracle | All | FINANCE | FINANCE | From SecLists/cirt.net archive |
| Oracle | Oracle | All | FND | FND | From SecLists/cirt.net archive |
| Oracle | Oracle | All | FROSTY | SNOWMAN | From SecLists/cirt.net archive |
| Oracle | Oracle | All | GL | GL | From SecLists/cirt.net archive |
| Oracle | Oracle | All | GPFD | GPFD | From SecLists/cirt.net archive |
| Oracle | Oracle | All | GPLD | GPLD | From SecLists/cirt.net archive |
| Oracle | Oracle | All | HCPARK | HCPARK | From SecLists/cirt.net archive |
| Oracle | Oracle | All | HLW | HLW | From SecLists/cirt.net archive |
| Oracle | Oracle | All | HR | HR | From SecLists/cirt.net archive |
| Oracle | Oracle | All | IMAGEUSER | IMAGEUSER | From SecLists/cirt.net archive |
| Oracle | Oracle | All | IMEDIA | IMEDIA | From SecLists/cirt.net archive |
| Oracle | Oracle | All | JMUSER | JMUSER | From SecLists/cirt.net archive |
| Oracle | Oracle | All | JONES | STEEL | From SecLists/cirt.net archive |
| Oracle | Oracle | All | JWARD | AIROPLANE | From SecLists/cirt.net archive |
| Oracle | Oracle | All | L2LDEMO | L2LDEMO | From SecLists/cirt.net archive |
| Oracle | Oracle | All | LBACSYS | LBACSYS | From SecLists/cirt.net archive |
| Oracle | Oracle | All | LIBRARIAN | SHELVES | From SecLists/cirt.net archive |
| Oracle | Oracle | All | MASTER | PASSWORD | From SecLists/cirt.net archive |
| Oracle | Oracle | All | MDDEMO | MDDEMO | From SecLists/cirt.net archive |
| Oracle | Oracle | All | MDDEMO_CLERK | CLERK | From SecLists/cirt.net archive |
| Oracle | Oracle | All | MDDEMO_MGR | MGR | From SecLists/cirt.net archive |
| Oracle | Oracle | All | MDSYS | MDSYS | From SecLists/cirt.net archive |
| Oracle | Oracle | All | MFG | MFG | From SecLists/cirt.net archive |
| Oracle | Oracle | All | MGWUSER | MGWUSER | From SecLists/cirt.net archive |
| Oracle | Oracle | All | MIGRATE | MIGRATE | From SecLists/cirt.net archive |
| Oracle | Oracle | All | MILLER | MILLER | From SecLists/cirt.net archive |
| Oracle | Oracle | All | MMO2 | MMO2 | From SecLists/cirt.net archive |
| Oracle | Oracle | All | MODTEST | YES | From SecLists/cirt.net archive |
| Oracle | Oracle | All | MOREAU | MOREAU | From SecLists/cirt.net archive |
| Oracle | Oracle | All | MTSSYS | MTSSYS | From SecLists/cirt.net archive |
| Oracle | Oracle | All | MTS_USER | MTS_PASSWORD | From SecLists/cirt.net archive |
| Oracle | Oracle | All | MTYSYS | MTYSYS | From SecLists/cirt.net archive |
| Oracle | Oracle | All | MXAGENT | MXAGENT | From SecLists/cirt.net archive |
| Oracle | Oracle | All | NAMES | NAMES | From SecLists/cirt.net archive |
| Oracle | Oracle | All | OAS_PUBLIC | OAS_PUBLIC | From SecLists/cirt.net archive |
| Oracle | Oracle | All | OCITEST | OCITEST | From SecLists/cirt.net archive |
| Oracle | Oracle | All | ODM | ODM | From SecLists/cirt.net archive |
| Oracle | Oracle | All | ODM_MTR | MTRPW | From SecLists/cirt.net archive |
| Oracle | Oracle | All | ODS | ODS | From SecLists/cirt.net archive |
| Oracle | Oracle | All | ODSCOMMON | ODSCOMMON | From SecLists/cirt.net archive |
| Oracle | Oracle | All | OE | OE | From SecLists/cirt.net archive |
| Oracle | Oracle | All | OEMADM | OEMADM | From SecLists/cirt.net archive |
| Oracle | Oracle | All | OEMREP | OEMREP | From SecLists/cirt.net archive |
| Oracle | Oracle | All | OLAPDBA | OLAPDBA | From SecLists/cirt.net archive |
| Oracle | Oracle | All | OLAPSVR | INSTANCE | From SecLists/cirt.net archive |
| Oracle | Oracle | All | OLAPSYS | MANAGER | From SecLists/cirt.net archive |
| Oracle | Oracle | All | OMWB_EMULATION | ORACLE | From SecLists/cirt.net archive |
| Oracle | Oracle | All | OO | OO | From SecLists/cirt.net archive |
| Oracle | Oracle | All | OPENSPIRIT | OPENSPIRIT | From SecLists/cirt.net archive |
| Oracle | Oracle | All | ORACACHE | (random password) | From SecLists/cirt.net archive |
| Oracle | Oracle | All | ORAREGSYS | ORAREGSYS | From SecLists/cirt.net archive |
| Oracle | Oracle | All | ORASSO | ORASSO | From SecLists/cirt.net archive |
| Oracle | Oracle | All | ORDPLUGINS | ORDPLUGINS | From SecLists/cirt.net archive |
| Oracle | Oracle | All | ORDSYS | ORDSYS | From SecLists/cirt.net archive |
| Oracle | Oracle | All | OSE$HTTP$ADMIN | (random password) | From SecLists/cirt.net archive |
| Oracle | Oracle | All | OSP22 | OSP22 | From SecLists/cirt.net archive |
| Oracle | Oracle | All | OUTLN | OUTLN | From SecLists/cirt.net archive |
| Oracle | Oracle | All | OWA | OWA | From SecLists/cirt.net archive |
| Oracle | Oracle | All | OWA_PUBLIC | OWA_PUBLIC | From SecLists/cirt.net archive |
| Oracle | Oracle | All | OWNER | OWNER | From SecLists/cirt.net archive |
| Oracle | Oracle | All | PANAMA | PANAMA | From SecLists/cirt.net archive |
| Oracle | Oracle | All | PATROL | PATROL | From SecLists/cirt.net archive |
| Oracle | Oracle | All | PERFSTAT | PERFSTAT | From SecLists/cirt.net archive |
| Oracle | Oracle | All | PLEX | PLEX | From SecLists/cirt.net archive |
| Oracle | Oracle | All | PLSQL | SUPERSECRET | From SecLists/cirt.net archive |
| Oracle | Oracle | All | PM | PM | From SecLists/cirt.net archive |
| Oracle | Oracle | All | PO | PO | From SecLists/cirt.net archive |
| Oracle | Oracle | All | PO7 | PO7 | From SecLists/cirt.net archive |
| Oracle | Oracle | All | PO8 | PO8 | From SecLists/cirt.net archive |
| Oracle | Oracle | All | PORTAL30 | PORTAL30 | From SecLists/cirt.net archive |
| Oracle | Oracle | All | PORTAL30 | PORTAL31 | From SecLists/cirt.net archive |
| Oracle | Oracle | All | PORTAL30_DEMO | PORTAL30_DEMO | From SecLists/cirt.net archive |
| Oracle | Oracle | All | PORTAL30_PUBLIC | PORTAL30_PUBLIC | From SecLists/cirt.net archive |
| Oracle | Oracle | All | PORTAL30_SSO | PORTAL30_SSO | From SecLists/cirt.net archive |
| Oracle | Oracle | All | PORTAL30_SSO_PS | PORTAL30_SSO_PS | From SecLists/cirt.net archive |
| Oracle | Oracle | All | PORTAL30_SSO_PUBLIC | PORTAL30_SSO_PUBLIC | From SecLists/cirt.net archive |
| Oracle | Oracle | All | POWERCARTUSER | POWERCARTUSER | From SecLists/cirt.net archive |
| Oracle | Oracle | All | PRIMARY | PRIMARY | From SecLists/cirt.net archive |
| Oracle | Oracle | All | PUBSUB | PUBSUB | From SecLists/cirt.net archive |
| Oracle | Oracle | All | PUBSUB1 | PUBSUB1 | From SecLists/cirt.net archive |
| Oracle | Oracle | All | QDBA | QDBA | From SecLists/cirt.net archive |
| Oracle | Oracle | All | QS | QS | From SecLists/cirt.net archive |
| Oracle | Oracle | All | QS_ADM | QS_ADM | From SecLists/cirt.net archive |
| Oracle | Oracle | All | QS_CB | QS_CB | From SecLists/cirt.net archive |
| Oracle | Oracle | All | QS_CBADM | QS_CBADM | From SecLists/cirt.net archive |
| Oracle | Oracle | All | QS_CS | QS_CS | From SecLists/cirt.net archive |
| Oracle | Oracle | All | QS_ES | QS_ES | From SecLists/cirt.net archive |
| Oracle | Oracle | All | QS_OS | QS_OS | From SecLists/cirt.net archive |
| Oracle | Oracle | All | QS_WS | QS_WS | From SecLists/cirt.net archive |
| Oracle | Oracle | All | RE | RE | From SecLists/cirt.net archive |
| Oracle | Oracle | All | REPADMIN | REPADMIN | From SecLists/cirt.net archive |
| Oracle | Oracle | All | REPORTS_USER | OEM_TEMP | From SecLists/cirt.net archive |
| Oracle | Oracle | All | REP_MANAGER | DEMO | From SecLists/cirt.net archive |
| Oracle | Oracle | All | REP_OWNER | DEMO | From SecLists/cirt.net archive |
| Oracle | Oracle | All | REP_OWNER | REP_OWNER | From SecLists/cirt.net archive |
| Oracle | Oracle | All | RMAIL | RMAIL | From SecLists/cirt.net archive |
| Oracle | Oracle | All | RMAN | RMAN | From SecLists/cirt.net archive |
| Oracle | Oracle | All | SAMPLE | SAMPLE | From SecLists/cirt.net archive |
| Oracle | Oracle | All | SAP | SAPR3 | From SecLists/cirt.net archive |
| Oracle | Oracle | All | SCOTT | TIGER | From SecLists/cirt.net archive |
| Oracle | Oracle | All | SDOS_ICSAP | SDOS_ICSAP | From SecLists/cirt.net archive |
| Oracle | Oracle | All | SECDEMO | SECDEMO | From SecLists/cirt.net archive |
| Oracle | Oracle | All | SERVICECONSUMER1 | SERVICECONSUMER1 | From SecLists/cirt.net archive |
| Oracle | Oracle | All | SH | SH | From SecLists/cirt.net archive |
| Oracle | Oracle | All | SITEMINDER | SITEMINDER | From SecLists/cirt.net archive |
| Oracle | Oracle | All | SLIDE | SLIDEPW | From SecLists/cirt.net archive |
| Oracle | Oracle | All | STARTER | STARTER | From SecLists/cirt.net archive |
| Oracle | Oracle | All | STRAT_USER | STRAT_PASSWD | From SecLists/cirt.net archive |
| Oracle | Oracle | All | SWPRO | SWPRO | From SecLists/cirt.net archive |
| Oracle | Oracle | All | SWUSER | SWUSER | From SecLists/cirt.net archive |
| Oracle | Oracle | All | SYMPA | SYMPA | From SecLists/cirt.net archive |
| Oracle | Oracle | All | SYS | CHANGE_ON_INSTALL | From SecLists/cirt.net archive |
| Oracle | Oracle | All | SYS | D_SYSPW | From SecLists/cirt.net archive |
| Oracle | Oracle | All | SYSADM | SYSADM | From SecLists/cirt.net archive |
| Oracle | Oracle | All | SYSMAN | OEM_TEMP | From SecLists/cirt.net archive |
| Oracle | Oracle | All | SYSTEM | D_SYSTPW | From SecLists/cirt.net archive |
| Oracle | Oracle | All | SYSTEM | MANAGER | From SecLists/cirt.net archive |
| Oracle | Oracle | All | TAHITI | TAHITI | From SecLists/cirt.net archive |
| Oracle | Oracle | All | TDOS_ICSAP | TDOS_ICSAP | From SecLists/cirt.net archive |
| Oracle | Oracle | All | TESTPILOT | TESTPILOT | From SecLists/cirt.net archive |
| Oracle | Oracle | All | TRACESRV | TRACE | From SecLists/cirt.net archive |
| Oracle | Oracle | All | TRACESVR | TRACE | From SecLists/cirt.net archive |
| Oracle | Oracle | All | TRAVEL | TRAVEL | From SecLists/cirt.net archive |
| Oracle | Oracle | All | TSDEV | TSDEV | From SecLists/cirt.net archive |
| Oracle | Oracle | All | TSUSER | TSUSER | From SecLists/cirt.net archive |
| Oracle | Oracle | All | TURBINE | TURBINE | From SecLists/cirt.net archive |
| Oracle | Oracle | All | ULTIMATE | ULTIMATE | From SecLists/cirt.net archive |
| Oracle | Oracle | All | USER | USER | From SecLists/cirt.net archive |
| Oracle | Oracle | All | USER0 | USER0 | From SecLists/cirt.net archive |
| Oracle | Oracle | All | USER1 | USER1 | From SecLists/cirt.net archive |
| Oracle | Oracle | All | USER2 | USER2 | From SecLists/cirt.net archive |
| Oracle | Oracle | All | USER3 | USER3 | From SecLists/cirt.net archive |
| Oracle | Oracle | All | USER4 | USER4 | From SecLists/cirt.net archive |
| Oracle | Oracle | All | USER5 | USER5 | From SecLists/cirt.net archive |
| Oracle | Oracle | All | USER6 | USER6 | From SecLists/cirt.net archive |
| Oracle | Oracle | All | USER7 | USER7 | From SecLists/cirt.net archive |
| Oracle | Oracle | All | USER8 | USER8 | From SecLists/cirt.net archive |
| Oracle | Oracle | All | USER9 | USER9 | From SecLists/cirt.net archive |
| Oracle | Oracle | All | UTLBSTATU | UTLESTAT | From SecLists/cirt.net archive |
| Oracle | Oracle | All | VIDEOUSER | VIDEO USER | From SecLists/cirt.net archive |
| Oracle | Oracle | All | VIF_DEVELOPER | VIF_DEV_PWD | From SecLists/cirt.net archive |
| Oracle | Oracle | All | VIRUSER | VIRUSER | From SecLists/cirt.net archive |
| Oracle | Oracle | All | VRR1 | VRR1 | From SecLists/cirt.net archive |
| Oracle | Oracle | All | WEBCAL01 | WEBCAL01 | From SecLists/cirt.net archive |
| Oracle | Oracle | All | WEBDB | WEBDB | From SecLists/cirt.net archive |
| Oracle | Oracle | All | WEBREAD | WEBREAD | From SecLists/cirt.net archive |
| Oracle | Oracle | All | WKSYS | WKSYS | From SecLists/cirt.net archive |
| Oracle | Oracle | All | WWW | WWW | From SecLists/cirt.net archive |
| Oracle | Oracle | All | WWWUSER | WWWUSER | From SecLists/cirt.net archive |
| Oracle | Oracle | All | XPRT | XPRT | From SecLists/cirt.net archive |
| Oracle | Oracle | All | admin | admin | http://docs.oracle.com/cd/E22630_01/Platform.1002/pdf/ATGInstallGuide.pdf |
| Oracle | Oracle | All | admin | adminadmin | http://www.oracle.com/technetwork/java/install-139173.html |
| Oracle | Oracle | All | admin | security | From SecLists/cirt.net archive |
| Oracle | Oracle | All | bpel | bpel | From SecLists/cirt.net archive |
| Oracle | Oracle | All | cn=orcladmin | welcome | From SecLists/cirt.net archive |
| Oracle | Oracle | All | ilom-admin | ilom-admin | http://seclists.org/fulldisclosure/2012/Nov/229 |
| Oracle | Oracle | All | ilom-operator | ilom-operator | http://seclists.org/fulldisclosure/2012/Nov/229 |
| Oracle | Oracle | All | internal | oracle | From SecLists/cirt.net archive |
| Oracle | Oracle | All | joe | password | From SecLists/cirt.net archive |
| Oracle | Oracle | All | mary | password | From SecLists/cirt.net archive |
| Oracle | Oracle | All | nm2user | nm2user | http://seclists.org/fulldisclosure/2012/Nov/229 |
| Oracle | Oracle | All | oracle | oracle | From SecLists/cirt.net archive |
| Oracle | Oracle | All | scott | tiger or tigger | From SecLists/cirt.net archive |
| Oracle | Oracle | All | siteadmin | siteadmin | http://docs.oracle.com/cd/E24152_01/Platform.10-1/ATGMultisiteAdminGuide/html/s1505accesscontrol01.html |
| Oracle | Oracle | All | sys | sys | From SecLists/cirt.net archive |
| Oracle | Oracle | All | system | password | From SecLists/cirt.net archive |
| Oracle | Oracle | All | system | security | From SecLists/cirt.net archive |
| Oracle | Oracle | All | system/manager | sys/change_on_install | From SecLists/cirt.net archive |
| Oracle | Oracle | All | weblogic | weblogic | From SecLists/cirt.net archive |
| Oracle | Oracle | All | wlcsystem | wlcsystem | From SecLists/cirt.net archive |
| Oracle | Oracle | All | wlpisystem | wlpisystem | From SecLists/cirt.net archive |
| PostgreSQL | PostgreSQL | All | postgres | (blank) | From SecLists/cirt.net archive |
| Sybase | Sybase | All | 12.x | (blank) | From SecLists/cirt.net archive |
| Sybase | Sybase | All | DBA | SQL | From SecLists/cirt.net archive |
| Sybase | Sybase | All | jagadmin | (blank) | From SecLists/cirt.net archive |
| Sybase | Sybase | All | sa | (blank) | From SecLists/cirt.net archive |
| Sybase | Sybase | All | sa | sasasa | From SecLists/cirt.net archive |
| Aris (mssql) | Aris (mssql) | All | ARIS9 | *ARIS!1dm9n# | From SecLists/cirt.net archive |
| Cassandra | Cassandra | All | cassandra | cassandra | From SecLists/cirt.net archive |
| CCH (mssql) | CCH (mssql) | All | sa | PracticeUser1 | From SecLists/cirt.net archive |
| Couchbase (web) | Couchbase (web) | All | Administrator | password | From SecLists/cirt.net archive |
| Couchdb | Couchdb | All | admin | password | From SecLists/cirt.net archive |
| db2 (db2) | db2 (db2) | All | ADONIS | BPMS | From SecLists/cirt.net archive |
| db2 (db2) | db2 (db2) | All | dasusr1 | dasusr1 | From SecLists/cirt.net archive |
| db2 (db2) | db2 (db2) | All | db2admin | db2admin | From SecLists/cirt.net archive |
| db2 (db2) | db2 (db2) | All | db2fenc1 | db2fenc1 | From SecLists/cirt.net archive |
| db2 (db2) | db2 (db2) | All | db2inst1 | db2inst1 | From SecLists/cirt.net archive |
| db2 (db2) | db2 (db2) | All | db2inst1 | db2pass | From SecLists/cirt.net archive |
| db2 (db2) | db2 (db2) | All | db2inst1 | db2password | From SecLists/cirt.net archive |
| db2 (db2) | db2 (db2) | All | db2inst1 | db2pw | From SecLists/cirt.net archive |
| easyWinArt (mssql) | easyWinArt (mssql) | All | sa | $easyWinArt4 | From SecLists/cirt.net archive |
| Elasticsearch (web) | Elasticsearch (web) | All | (blank) | (blank) | From SecLists/cirt.net archive |
| elasticsearch (web) | elasticsearch (web) | All | elastic | changeme | From SecLists/cirt.net archive |
| Emerson AMS (mssql) | Emerson AMS (mssql) | All | sa | 42Emerson42Eme | From SecLists/cirt.net archive |
| GeoNetwork (mssql) | GeoNetwork (mssql) | All | admin | gnos | From SecLists/cirt.net archive |
| i2b2 Workbench (mssql) | i2b2 Workbench (mssql) | All | I2b2demodata2 | i2b2demodata2 | From SecLists/cirt.net archive |
| i2b2 Workbench (mssql) | i2b2 Workbench (mssql) | All | I2b2demodata | i2b2demodata | From SecLists/cirt.net archive |
| i2b2 Workbench (mssql) | i2b2 Workbench (mssql) | All | I2b2hive | i2b2hive | From SecLists/cirt.net archive |
| i2b2 Workbench (mssql) | i2b2 Workbench (mssql) | All | I2b2metadata2 | i2b2metadata2 | From SecLists/cirt.net archive |
| i2b2 Workbench (mssql) | i2b2 Workbench (mssql) | All | I2b2metadata | i2b2metadata | From SecLists/cirt.net archive |
| i2b2 Workbench (mssql) | i2b2 Workbench (mssql) | All | I2b2workdata2 | i2b2workdata2 | From SecLists/cirt.net archive |
| i2b2 Workbench (mssql) | i2b2 Workbench (mssql) | All | I2b2workdata | i2b2workdata | From SecLists/cirt.net archive |
| IBM Maximo (mssql) | IBM Maximo (mssql) | All | maxadmin | maxadmin | From SecLists/cirt.net archive |
| IBM Maximo (mssql) | IBM Maximo (mssql) | All | maxreg | maxreg | From SecLists/cirt.net archive |
| IBM Maximo (mssql) | IBM Maximo (mssql) | All | mxintadm | mxintadm | From SecLists/cirt.net archive |
| IBM WAS (mssql) | IBM WAS (mssql) | All | wasadmin | wasadmin | From SecLists/cirt.net archive |
| IHS Kingdom (mssql) | IHS Kingdom (mssql) | All | sa | $ei$micMicro | From SecLists/cirt.net archive |
| InfluxDB (web) | InfluxDB (web) | All | admin | admin | From SecLists/cirt.net archive |
| Lasa AIMS (mssql) | Lasa AIMS (mssql) | All | ADMIN | AIMS | From SecLists/cirt.net archive |
| Lasa AIMS (mssql) | Lasa AIMS (mssql) | All | FB | AIMS | From SecLists/cirt.net archive |
| Lenel OnGuard (mssql) | Lenel OnGuard (mssql) | All | LENEL | MULTIMEDIA | From SecLists/cirt.net archive |
| MediaPortal (mssql) | MediaPortal (mssql) | All | sa | M3d!aP0rtal | From SecLists/cirt.net archive |
| medo.check (mssql) | medo.check (mssql) | All | mcUser | medocheck123 | From SecLists/cirt.net archive |
| Micro Focus Silk Central (mssql) | Micro Focus Silk Central (mssql) | All | sa | SilkCentral12!34 | From SecLists/cirt.net archive |
| Mongodb noauth (mongodb) | Mongodb noauth (mongodb) | All | (blank) | (blank) | From SecLists/cirt.net archive |
| Mongo Express (web) | Mongo Express (web) | All | admin | pass | From SecLists/cirt.net archive |
| Mongo Express (web) | Mongo Express (web) | All | (blank) | (blank) | From SecLists/cirt.net archive |
| MSSQL (mssql) | MSSQL (mssql) | All | ADONI | BPMS | From SecLists/cirt.net archive |
| MSSQL (mssql) | MSSQL (mssql) | All | sa | (blank) | From SecLists/cirt.net archive |
| MSSQL (mssql) | MSSQL (mssql) | All | sa | password | From SecLists/cirt.net archive |
| MSSQL (mssql) | MSSQL (mssql) | All | sa | Password123 | From SecLists/cirt.net archive |
| MSSQL (mssql) | MSSQL (mssql) | All | sa | sa | From SecLists/cirt.net archive |
| MSSQL (mssql) | MSSQL (mssql) | All | sa | sqlserver | From SecLists/cirt.net archive |
| MySQL (ssh) | MySQL (ssh) | All | root | root | From SecLists/cirt.net archive |
| Napco Continental Access (mssql) | Napco Continental Access (mssql) | All | cic | cic | From SecLists/cirt.net archive |
| Napco Continental Access (mssql) | Napco Continental Access (mssql) | All | cic | cic!23456789 | From SecLists/cirt.net archive |
| Napco Continental Access (mssql) | Napco Continental Access (mssql) | All | sa | cic | From SecLists/cirt.net archive |
| Napco Continental Access (mssql) | Napco Continental Access (mssql) | All | sa | cic!23456789 | From SecLists/cirt.net archive |
| Neo4j | Neo4j | All | neo4j | neo4j | From SecLists/cirt.net archive |
| NetXMS (mssql) | NetXMS (mssql) | All | admin | netxms | From SecLists/cirt.net archive |
| OpenGTS (mssql) | OpenGTS (mssql) | All | gts | opengts | From SecLists/cirt.net archive |
| Oracle | Oracle | All | (blank) | (blank) | From SecLists/cirt.net archive |
| Oracle Glassfish (web) | Oracle Glassfish (web) | All | admin | admin | From SecLists/cirt.net archive |
| Oracle Glassfish (web) | Oracle Glassfish (web) | All | admin | (blank) | From SecLists/cirt.net archive |
| postgres (postgres) | postgres (postgres) | All | admin | admin | From SecLists/cirt.net archive |
| postgres (postgres) | postgres (postgres) | All | admin | password | From SecLists/cirt.net archive |
| postgres (postgres) | postgres (postgres) | All | dcmadmin | passw0rd | From SecLists/cirt.net archive |
| postgres (postgres) | postgres (postgres) | All | postgres | 123 | From SecLists/cirt.net archive |
| postgres (postgres) | postgres (postgres) | All | postgres | admin | From SecLists/cirt.net archive |
| postgres (postgres) | postgres (postgres) | All | postgres | amber | From SecLists/cirt.net archive |
| postgres (postgres) | postgres (postgres) | All | postgres | password | From SecLists/cirt.net archive |
| postgres (postgres) | postgres (postgres) | All | postgres | postgres | From SecLists/cirt.net archive |
| Redis (redis) | Redis (redis) | All | (blank) | (blank) | From SecLists/cirt.net archive |
| SafeNet Sentinel EMS (mssql) | SafeNet Sentinel EMS (mssql) | All | sa | DBA!sa@EMSDB123 | From SecLists/cirt.net archive |
| Schlage SMS (mssql) | Schlage SMS (mssql) | All | sa | SECAdmin1 | From SecLists/cirt.net archive |
| Schlage SMS (mssql) | Schlage SMS (mssql) | All | SMSAdmin | SECAdmin1 | From SecLists/cirt.net archive |
| Scrutinizer (MySQL) | Scrutinizer (MySQL) | All | scrutremote | admin | From SecLists/cirt.net archive |
| SKF @ptitude Analyst (mssql) | SKF @ptitude Analyst (mssql) | All | sa | skf_admin1 | From SecLists/cirt.net archive |
| SplendidCRM (mssql) | SplendidCRM (mssql) | All | sa | splendidcrm2005 | From SecLists/cirt.net archive |
| Telestream Vantage (mssql) | Telestream Vantage (mssql) | All | sa | vantage12! | From SecLists/cirt.net archive |
| TimeForce (mssql) | TimeForce (mssql) | All | sa | dr8gedog | From SecLists/cirt.net archive |
| UTC FCWnx (mssql) | UTC FCWnx (mssql) | All | sa | SecurityMaster08 | From SecLists/cirt.net archive |
| Video Insight (mssql) | Video Insight (mssql) | All | sa | V4in$ight | From SecLists/cirt.net archive |
| WelchAllyn CardioPerfect (mssql) | WelchAllyn CardioPerfect (mssql) | All | sa | Cardio.Perfect | From SecLists/cirt.net archive |
| Wonderware Historian (mssql) | Wonderware Historian (mssql) | All | aaAdmin | pwAdmin | From SecLists/cirt.net archive |
| Wonderware Historian (mssql) | Wonderware Historian (mssql) | All | aadbo | pwddbo | From SecLists/cirt.net archive |
| Wonderware Historian (mssql) | Wonderware Historian (mssql) | All | aaPower | pwPower | From SecLists/cirt.net archive |
| Wonderware Historian (mssql) | Wonderware Historian (mssql) | All | aaUser | pwUser | From SecLists/cirt.net archive |
| Wonderware Historian (mssql) | Wonderware Historian (mssql) | All | wwAdmin | wwAdmin | From SecLists/cirt.net archive |
| Wonderware Historian (mssql) | Wonderware Historian (mssql) | All | wwdbo | wwdbo | From SecLists/cirt.net archive |
| Wonderware Historian (mssql) | Wonderware Historian (mssql) | All | wwPower | wwPower | From SecLists/cirt.net archive |
| Wonderware Historian (mssql) | Wonderware Historian (mssql) | All | wwUser | wwUser | From SecLists/cirt.net archive |

## 7. Application servers / middleware

| Product | Vendor | Version(s) | Username | Password | Notes |
|---|---|---|---|---|---|
| Lucee Server admin | Lucee | All | (blank) | (set on install) | Web admin |
| ColdFusion Administrator | Adobe | All | admin | (set on install) | Web admin |
| Jetty | Eclipse | All | admin | admin | Demo realm only |
| GlassFish | Oracle | All | admin | adminadmin | Older installer |
| GlassFish | Oracle | All | admin | (blank) | Web admin |
| WebSphere Application Server | IBM | All | wasadmin | wasadmin | ISC |
| WebSphere Application Server | IBM | All | admin | admin | ISC/wsadmin |
| WebLogic Server | Oracle | All | system | manager | Older default |
| WebLogic Server | Oracle | All | weblogic | welcome1 | Common install default |
| WebLogic Server | Oracle | All | weblogic | weblogic | Older default |
| WildFly Management | Red Hat | All | (set via add-user.sh) | (set via add-user.sh) | Must run add-user script |
| JBoss EAP/AS | Red Hat | <7 | admin | admin | JMX/admin-console |
| Tomcat Host Manager | Apache | All | admin | (blank) | host-manager role |
| Tomcat Manager | Apache | All | manager | manager | Common install default |
| Tomcat Manager | Apache | All | admin | admin | Common install default |
| Tomcat Manager | Apache | All | tomcat | tomcat | Web manager; not enabled by default |
| Apache Project | Apache Project | All | jj | (blank) | From SecLists/cirt.net archive |
| weblogic | weblogic | All | system | weblogic | From SecLists/cirt.net archive |
| Apache guacamole | Apache guacamole | All | guacadmin | guacadmin | From SecLists/cirt.net archive |
| Apache Tomcat Host Manager (web) | Apache Tomcat Host Manager (web) | All | admin | admin | From SecLists/cirt.net archive |
| Apache Tomcat Host Manager (web) | Apache Tomcat Host Manager (web) | All | admin | (blank) | From SecLists/cirt.net archive |
| Apache Tomcat Host Manager (web) | Apache Tomcat Host Manager (web) | All | admin | j5Brn9 | From SecLists/cirt.net archive |
| Apache Tomcat Host Manager (web) | Apache Tomcat Host Manager (web) | All | admin | tomcat | From SecLists/cirt.net archive |
| Apache Tomcat Host Manager (web) | Apache Tomcat Host Manager (web) | All | cxsdk | kdsxc | From SecLists/cirt.net archive |
| Apache Tomcat Host Manager (web) | Apache Tomcat Host Manager (web) | All | j2deployer | j2deployer | From SecLists/cirt.net archive |
| Apache Tomcat Host Manager (web) | Apache Tomcat Host Manager (web) | All | ovwebusr | OvW*busr1 | From SecLists/cirt.net archive |
| Apache Tomcat Host Manager (web) | Apache Tomcat Host Manager (web) | All | QCC | QLogic66 | From SecLists/cirt.net archive |
| Apache Tomcat Host Manager (web) | Apache Tomcat Host Manager (web) | All | role1 | role1 | From SecLists/cirt.net archive |
| Apache Tomcat Host Manager (web) | Apache Tomcat Host Manager (web) | All | role1 | tomcat | From SecLists/cirt.net archive |
| Apache Tomcat Host Manager (web) | Apache Tomcat Host Manager (web) | All | role | changethis | From SecLists/cirt.net archive |
| Apache Tomcat Host Manager (web) | Apache Tomcat Host Manager (web) | All | root | root | From SecLists/cirt.net archive |
| Apache Tomcat Host Manager (web) | Apache Tomcat Host Manager (web) | All | tomcat | changethis | From SecLists/cirt.net archive |
| Apache Tomcat Host Manager (web) | Apache Tomcat Host Manager (web) | All | tomcat | s3cret | From SecLists/cirt.net archive |
| Apache Tomcat Host Manager (web) | Apache Tomcat Host Manager (web) | All | tomcat | tomcat | From SecLists/cirt.net archive |
| Apache Tomcat Host Manager (web) | Apache Tomcat Host Manager (web) | All | xampp | xampp | From SecLists/cirt.net archive |
| JBoss AS 6 Alt (web) | JBoss AS 6 Alt (web) | All | admin | admin | From SecLists/cirt.net archive |
| JBoss AS 6 (web) | JBoss AS 6 (web) | All | admin | admin | From SecLists/cirt.net archive |
| Weblogic (web) | Weblogic (web) | All | EXAMPLES | EXAMPLES | From SecLists/cirt.net archive |
| Weblogic (web) | Weblogic (web) | All | monitor | password | From SecLists/cirt.net archive |
| Weblogic (web) | Weblogic (web) | All | operator | password | From SecLists/cirt.net archive |
| Weblogic (web) | Weblogic (web) | All | operator | weblogic | From SecLists/cirt.net archive |
| Weblogic (web) | Weblogic (web) | All | PUBLIC | PUBLIC | From SecLists/cirt.net archive |
| Weblogic (web) | Weblogic (web) | All | system | manager | From SecLists/cirt.net archive |
| Weblogic (web) | Weblogic (web) | All | system | Passw0rd | From SecLists/cirt.net archive |
| Weblogic (web) | Weblogic (web) | All | system | password | From SecLists/cirt.net archive |
| Weblogic (web) | Weblogic (web) | All | system | welcome(1) | From SecLists/cirt.net archive |
| Weblogic (web) | Weblogic (web) | All | weblogic | weblogic | From SecLists/cirt.net archive |
| Weblogic (web) | Weblogic (web) | All | weblogic | weblogic1 | From SecLists/cirt.net archive |
| Weblogic (web) | Weblogic (web) | All | weblogic | welcome(1) | From SecLists/cirt.net archive |
| WebSphere (web) | WebSphere (web) | All | system | manager | From SecLists/cirt.net archive |

## 8. CI/CD & DevOps

| Product | Vendor | Version(s) | Username | Password | Notes |
|---|---|---|---|---|---|
| Spinnaker Deck | Netflix/OSS | All | (no auth) | (no auth) | Default has no auth |
| Concourse CI | Concourse | All | test | test | Web admin in dev mode |
| Drone CI | Drone | All | (OAuth via SCM) | (OAuth via SCM) | No local default |
| ArgoCD | Argo | All | admin | (generated, in argocd-initial-admin-secret) | Web admin |
| Octopus Deploy | Octopus | All | (set on install) | (set on install) | Wizard; no shipped default |
| Ansible AWX/Tower | Red Hat | All | admin | password | Web admin |
| Rundeck | Rundeck | All | admin | admin | Web admin |
| Harbor Registry | VMware | All | admin | Harbor12345 | Web admin |
| Artifactory | JFrog | All | admin | password | Web admin; must change on first login |
| Nexus Repository | Sonatype | >=3.17 | admin | (generated, in admin.password file) | Must change on first login |
| Nexus Repository | Sonatype | <3.17 | admin | admin123 | Web admin |
| SonarQube | SonarSource | All | admin | admin | Web admin; must change on first login (newer) |
| TeamCity | JetBrains | All | (set on install) | (set on install) | Web wizard |
| Bamboo | Atlassian | All | admin | admin | Web admin |
| GitLab CE/EE | GitLab | >=14 | root | (generated, in /etc/gitlab/initial_root_password) | Web admin |
| Jenkins (post-setup wizard) | Jenkins | All | admin | admin | Common when wizard skipped |
| Jenkins | Jenkins | All | admin | (generated initial token) | Initial admin password printed at startup |
| Sonatype Nexus Repository Manager | Sonatype Nexus Repository Manager | All | admin | admin123 | https://help.sonatype.com/repomanager2/maven-and-other-build-tools/sbt |
| Sonatype Nexus Repository Manager | Sonatype Nexus Repository Manager | All | nexus | nexus | From SecLists/cirt.net archive |
| Artifactory | Artifactory | All | access-admin | password | From SecLists/cirt.net archive |
| Artifactory | Artifactory | All | access-admin | (random password) | From SecLists/cirt.net archive |
| Artifactory | Artifactory | All | admin | password | From SecLists/cirt.net archive |
| Artifactory | Artifactory | All | anonymous | (blank) | From SecLists/cirt.net archive |
| Drone CI (web) | Drone CI (web) | All | admin | admin | From SecLists/cirt.net archive |
| Gitlab | Gitlab | All | admin | 5iveL!fe | From SecLists/cirt.net archive |
| Gitlab | Gitlab | All | admin@local.host | 5iveL!fe | From SecLists/cirt.net archive |
| Gitlab | Gitlab | All | root | 5iveL!fe | From SecLists/cirt.net archive |
| Harbor (web) | Harbor (web) | All | admin | Harbor12345 | From SecLists/cirt.net archive |
| Jenkins (web) | Jenkins (web) | All | (blank) | (blank) | From SecLists/cirt.net archive |
| Nexus Repository Manager (web) | Nexus Repository Manager (web) | All | admin | admin123 | From SecLists/cirt.net archive |
| Rundeck (web) | Rundeck (web) | All | admin | admin | From SecLists/cirt.net archive |
| SonarQube (web) | SonarQube (web) | All | admin | admin | From SecLists/cirt.net archive |
| TeamCity 9 Guest (web) | TeamCity 9 Guest (web) | All | (blank) | (blank) | From SecLists/cirt.net archive |

## 9. Monitoring & logging

| Product | Vendor | Version(s) | Username | Password | Notes |
|---|---|---|---|---|---|
| op5 Monitor | op5 | All | monitor | monitor | Web admin |
| LibreNMS | LibreNMS | All | (set on install) | (set on install) | Web wizard |
| Observium | Observium | All | admin | admin | Web admin |
| Icinga Web 2 | Icinga | All | icingaadmin | icinga | Web admin |
| Prometheus | Prometheus | All | (no auth) | (no auth) | Default has no auth |
| Graylog | Graylog | All | admin | (set in graylog.conf) | Web admin (root_password_sha2) |
| Cacti | Cacti | All | admin | admin | Web admin; must change on first login |
| Centreon | Centreon | All | admin | centreon | Web admin |
| SolarWinds Orion | SolarWinds | All | admin | (blank) | Web admin |
| PRTG Network Monitor | Paessler | All | prtgadmin | prtgadmin | Web admin; must change on first login |
| Nagios Core | Nagios | All | nagiosadmin | (set in htpasswd) | Web admin |
| Nagios XI | Nagios | All | nagiosadmin | nagiosadmin | Web admin |
| Zabbix Guest | Zabbix | <5.2 | guest | (blank) | Read-only; removed in newer |
| Splunk Enterprise | Splunk | >=7.1 | admin | (set on install) | Must set during setup |
| Kibana | Elastic | <8 | (blank) | (blank) | No auth by default |
| Grafana | Grafana Labs | All | admin | admin | Web admin; must change on first login |
| PRTG | PRTG | All | prtgadmin | prtgadmin | From SecLists/cirt.net archive |
| SolarWinds | SolarWinds | All | LocalAdministrator | #l@$ak#.lk;0@P | http://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2004-2532 |
| SolarWinds | SolarWinds | All | whd | whd | http://www.solarwinds.com/documentation/WebHelpDesk/docs/WHDAdminGuide.pdf |
| SolarWinds | SolarWinds | All | admin | (blank) | From SecLists/cirt.net archive |
| Splunk | Splunk | All | admin | changeme | From SecLists/cirt.net archive |
| zabbix | zabbix | All | Admin | zabbix | From SecLists/cirt.net archive |
| Centreon WebUI | Centreon WebUI | All | admin | centreon | From SecLists/cirt.net archive |
| Grafana (general) | Grafana (general) | All | admin | admin | From SecLists/cirt.net archive |
| Graylog (web) | Graylog (web) | All | admin | admin | From SecLists/cirt.net archive |
| Kibana (web) | Kibana (web) | All | elastic | changeme | From SecLists/cirt.net archive |
| Nagios (web) | Nagios (web) | All | nagiosadmin | nagiosadmin | From SecLists/cirt.net archive |
| Zabbix (web) | Zabbix (web) | All | Admin | zabbix | From SecLists/cirt.net archive |

## 10. CMS & web platforms

| Product | Vendor | Version(s) | Username | Password | Notes |
|---|---|---|---|---|---|
| OpenCart Admin | OpenCart | All | admin | (set on install) | Web wizard |
| Adobe AEM | Adobe | All | admin | admin | OSGi/CRX admin |
| DotNetNuke (DNN) | DNN | All | host | dnnhost | Web admin |
| Sitecore | Sitecore | All | sitecore\admin | b | Web admin (older) |
| Sitecore | Sitecore | All | admin | b | Web admin (older) |
| Umbraco | Umbraco | All | admin | (set on install) | Web wizard |
| Bitnami stack | Bitnami | All | user | bitnami | Linux user / web admin |
| Jira (install) | Atlassian | All | admin | admin | Common dev install |
| Confluence (install) | Atlassian | All | admin | (set on install) | Web wizard |
| MediaWiki (install) | Wikimedia | All | WikiSysop | (set on install) | Web installer |
| phpMyAdmin | phpMyAdmin | All | pma | (blank) | Some shared-host installs |
| phpMyAdmin | phpMyAdmin | All | root | (MySQL root password) | Uses underlying MySQL creds |
| Magento Admin | Adobe/Magento | All | admin | (set on install) | Web admin |
| Drupal (install) | Drupal | All | admin | (set on install) | Web installer |
| Joomla! (install) | Joomla | All | admin | (set on install) | Web installer |
| WordPress (install) | WordPress | All | admin | (set on install) | Web installer; no shipped default |
| Magento | Magento | All | admin | 123123 | http://www.magentocommerce.com/wiki/recover/resetting-admin-password |
| Sitecore Corporation | Sitecore Corporation | All | Audrey | a | http://www.procheckup.com/media/176566/pentesting_sitecore.pdf |
| Sitecore Corporation | Sitecore Corporation | All | Bill | b | http://www.procheckup.com/media/176566/pentesting_sitecore.pdf |
| Sitecore Corporation | Sitecore Corporation | All | Denny | d | http://www.procheckup.com/media/176566/pentesting_sitecore.pdf |
| Sitecore Corporation | Sitecore Corporation | All | Lonnie | l | http://www.procheckup.com/media/176566/pentesting_sitecore.pdf |
| Sitecore Corporation | Sitecore Corporation | All | Minnie | m | http://www.procheckup.com/media/176566/pentesting_sitecore.pdf |
| Sitecore Corporation | Sitecore Corporation | All | admin | b | http://sdn.sitecore.net/upload/sdn5/tools/v53_to_v6/sitecore_cms_53_to_cms_6_database_conversion_tool-a4.pdf |
| TYPO3 | TYPO3 | All | (blank) | joh316 | From SecLists/cirt.net archive |
| TYPO3 | TYPO3 | All | admin | password | From SecLists/cirt.net archive |
| Typo3 Association | Typo3 Association | All | admin | password | From SecLists/cirt.net archive |
| drupal.org | drupal.org | All | admin | admin | From SecLists/cirt.net archive |
| phpMyAdmin | phpMyAdmin | All | root | (blank) | From SecLists/cirt.net archive |
| Atlassian Confluence | Atlassian Confluence | All | disabledsystemuser | disabled1system1user6708 | From SecLists/cirt.net archive |

## 11. Industrial / SCADA / OT / PLC

| Product | Vendor | Version(s) | Username | Password | Notes |
|---|---|---|---|---|---|
| Tridium Niagara | Tridium | All | admin | Niagara4 | Newer Niagara4 install |
| Tridium Niagara | Tridium | All | tridium | niagara | Web Workbench |
| Delta PLC DVP | Delta | All | (no auth) | (no auth) | Modbus open |
| Advantech ADAM | Advantech | All | 00000000 | 00000000 | Telnet/web |
| Moxa EDS switch | Moxa | All | admin | (blank) | Web admin |
| Phoenix Contact mGuard | Phoenix Contact | All | admin | mGuard | Web admin |
| Phoenix Contact ILC PLC | Phoenix Contact | All | admin | private | Web/FTP |
| Inductive Automation Ignition | Inductive Automation | All | admin | password | Web admin; must change on first login |
| Wonderware Historian | AVEVA/Wonderware | All | wwPower | wwPower | MSSQL backend |
| Wonderware Historian | AVEVA/Wonderware | All | wwUser | wwUser | MSSQL backend |
| Wonderware Historian | AVEVA/Wonderware | All | wwAdmin | wwAdmin | MSSQL backend |
| Wonderware InTouch | AVEVA/Wonderware | All | Administrator | Wonderware | HMI runtime |
| Yokogawa CENTUM VP | Yokogawa | All | CENTUM | CENTUM | Engineering |
| Honeywell Experion PKS | Honeywell | All | mngr | mngr | Engineering |
| GE Fanuc PLC | GE | All | (no auth) | (no auth) | SRTP open |
| ABB AC500 | ABB | All | Administrator | (blank) | Web/CoDeSys |
| Omron CJ/CP1 | Omron | All | (no auth) | (no auth) | FINS protocol open |
| Mitsubishi MELSEC iQ-R | Mitsubishi | All | (no auth) | (no auth) | MC protocol open |
| Schneider EcoStruxure | Schneider Electric | All | admin | admin | Web admin |
| Modicon Quantum | Schneider Electric | All | (blank) | (blank) | FTP open |
| FactoryTalk View SE | Rockwell | All | admin | admin | HMI |
| ControlLogix / CompactLogix | Allen-Bradley/Rockwell | All | (no auth) | (no auth) | EtherNet/IP open by default |
| SIMATIC PCS 7 | Siemens | All | Administrator | 0 | Service |
| SIMATIC HMI Panel | Siemens | All | Administrator | 100 | Service login |
| SIMATIC S7-1200/1500 | Siemens | All | (blank) | (blank) | No auth by default; PG/HMI must enable |
| Fujitsu Siemens | Fujitsu Siemens | All | (blank) | connect | From SecLists/cirt.net archive |
| Fujitsu Siemens | Fujitsu Siemens | All | manage | !manage | From SecLists/cirt.net archive |
| Honeywell | Honeywell | All | LocalComServer | LCS pwd 03 | From SecLists/cirt.net archive |
| Honeywell | Honeywell | All | TPSLocalServer | TLS pwd 03 | From SecLists/cirt.net archive |
| OMRON | OMRON | All | <N/A> | (blank) | From SecLists/cirt.net archive |
| Schneider Electric | Schneider Electric | All | (blank) | admin | From SecLists/cirt.net archive |
| Schneider Electric | Schneider Electric | All | USER | USER | From SecLists/cirt.net archive |
| Schneider Electric | Schneider Electric | All | ntpupdate | ntpupdate | From SecLists/cirt.net archive |
| Siemens | Siemens | All | 31994 | 31994 | From SecLists/cirt.net archive |
| Siemens | Siemens | All | (blank) | 0 | From SecLists/cirt.net archive |
| Siemens | Siemens | All | (blank) | 123456 | http://wiki.unify.com/wiki/OpenStage_SIP_FAQ#What_are_the_default_passwords.3F |
| Siemens | Siemens | All | (blank) | admin | From SecLists/cirt.net archive |
| Siemens | Siemens | All | <N/A> | 123456 | From SecLists/cirt.net archive |
| Siemens | Siemens | All | <N/A> | (blank) | From SecLists/cirt.net archive |
| Siemens | Siemens | All | <N/A> | SKY_FOX | From SecLists/cirt.net archive |
| Siemens | Siemens | All | <N/A> | admin | From SecLists/cirt.net archive |
| Siemens | Siemens | All | <N/A> | gubed | From SecLists/cirt.net archive |
| Siemens Corp | Siemens Corp | All | 18140815 | 18140815 | From SecLists/cirt.net archive |
| Siemens Corp | Siemens Corp | All | 31994 | 31994 | From SecLists/cirt.net archive |
| Siemens Corp | Siemens Corp | All | (blank) | SKY_FOX | From SecLists/cirt.net archive |
| Siemens Corp | Siemens Corp | All | (blank) | uboot | From SecLists/cirt.net archive |
| Siemens Corp | Siemens Corp | All | WinCCAdmin | 2WSXcde | http://iadt.siemens.ru/forum/viewtopic.php?p=2974&sid=58cedcf3a0fc7a0b6c61c7bc46530928 |
| Siemens Corp | Siemens Corp | All | WinCCConnect | 2WSXcder | http://iadt.siemens.ru/forum/viewtopic.php?p=2974&sid=58cedcf3a0fc7a0b6c61c7bc46530928 |
| Siemens Corp | Siemens Corp | All | admin | (blank) | From SecLists/cirt.net archive |
| Siemens Corp | Siemens Corp | All | admin | pwp | From SecLists/cirt.net archive |
| Siemens Corp | Siemens Corp | All | eng | engineer | From SecLists/cirt.net archive |
| Siemens Corp | Siemens Corp | All | op | op | From SecLists/cirt.net archive |
| Siemens Corp | Siemens Corp | All | op | operator | From SecLists/cirt.net archive |
| Siemens Corp | Siemens Corp | All | poll | poll | From SecLists/cirt.net archive |
| Siemens Corp | Siemens Corp | All | poll | tech | From SecLists/cirt.net archive |
| Siemens Corp | Siemens Corp | All | su | super | From SecLists/cirt.net archive |
| Siemens Corp | Siemens Corp | All | sysadmin | sysadmin | From SecLists/cirt.net archive |
| Siemens Corp | Siemens Corp | All | system | field | From SecLists/cirt.net archive |
| Siemens Corp | Siemens Corp | All | system | system | From SecLists/cirt.net archive |
| Siemens Corp | Siemens Corp | All | tech | tech | From SecLists/cirt.net archive |
| Siemens | Siemens | All | admin | (blank) | From SecLists/cirt.net archive |
| Siemens | Siemens | All | admin | <N/A> | From SecLists/cirt.net archive |
| Siemens | Siemens | All | admin | admin | Also has an account with: |
| Siemens | Siemens | All | admin | hagpolm1 | From SecLists/cirt.net archive |
| Siemens | Siemens | All | admin | pwp | From SecLists/cirt.net archive |
| Siemens | Siemens | All | basisk | basisk | http://m.itworld.com/data-centerservers/190269/power-plant-hack-anybody-could-use |
| Siemens | Siemens | All | eng | engineer | From SecLists/cirt.net archive |
| Siemens | Siemens | All | op | op | From SecLists/cirt.net archive |
| Siemens | Siemens | All | op | operator | From SecLists/cirt.net archive |
| Siemens | Siemens | All | poll | tech | From SecLists/cirt.net archive |
| Siemens | Siemens | All | su | super | From SecLists/cirt.net archive |
| Siemens | Siemens | All | superuser | admin | From SecLists/cirt.net archive |
| Siemens | Siemens | All | sysadmin | sysadmin | From SecLists/cirt.net archive |
| Siemens | Siemens | All | tech | field | From SecLists/cirt.net archive |
| Siemens | Siemens | All | tech | tech | From SecLists/cirt.net archive |
| Yokogawa | Yokogawa | All | <N/A> | 727 | For model codes ending in E |
| Yokogawa | Yokogawa | All | admin | !admin | TFGW410 ISA100 gateway |
| schneider | schneider | All | USER | USER | From SecLists/cirt.net archive |
| Fujitsu Siemens | Fujitsu Siemens | All | (blank) | fi-scanner | From SecLists/cirt.net archive |
| honeywell (ssh) | honeywell (ssh) | All | admin | 12345 | From SecLists/cirt.net archive |
| honeywell (web) | honeywell (web) | All | admin | 1234 | From SecLists/cirt.net archive |
| Moxa | Moxa | All | admin | moxa | From SecLists/cirt.net archive |
| Moxa | Moxa | All | (blank) | moxa | From SecLists/cirt.net archive |
| Moxa (telnet) (CVE-2016-8717) | Moxa (telnet) (CVE-2016-8717) | All | 94jo3dkru4 | moxaiwroot | From SecLists/cirt.net archive |
| OMRON | OMRON | All | (blank) | (blank) | From SecLists/cirt.net archive |
| RabbitMQ | RabbitMQ | All | guest | guest | From SecLists/cirt.net archive |
| Schneider Electric | Schneider Electric | All | Administrator | admin | From SecLists/cirt.net archive |
| Schneider M340(FTP) | Schneider M340(FTP) | All | sysdiag | factorycast@schneider | From SecLists/cirt.net archive |
| Schneider M340(Web) | Schneider M340(Web) | All | USER | USER | From SecLists/cirt.net archive |
| Schneider Premium(FTP) | Schneider Premium(FTP) | All | sysdiag | factorycast@schneider | From SecLists/cirt.net archive |
| Schneider Premium(WEB) | Schneider Premium(WEB) | All | USER | USER | From SecLists/cirt.net archive |
| Siemens | Siemens | All | (blank) | (blank) | From SecLists/cirt.net archive |
| Siemens | Siemens | All | (blank) | gubed | From SecLists/cirt.net archive |
| Siemens | Siemens | All | (blank) | SKY_FOX | From SecLists/cirt.net archive |
| Siemens S7-1200(Web) | Siemens S7-1200(Web) | All | admin | (blank) | From SecLists/cirt.net archive |
| siemens (web) | siemens (web) | All | admin | admin | From SecLists/cirt.net archive |
| Yokogawa | Yokogawa | All | (blank) | 727 | From SecLists/cirt.net archive |

## 12. IoT / smart-home / consumer

| Product | Vendor | Version(s) | Username | Password | Notes |
|---|---|---|---|---|---|
| Roku TV/Player | Roku | All | (no auth on ECP) | (no auth on ECP) | External Control Protocol open by default |
| Chromecast | Google | All | (no auth) | (no auth) | Local control via DIAL |
| Sonos speaker | Sonos | All | (no auth on local API) | (no auth on local API) | Local SOAP open |
| Wyze Cam | Wyze | All | (cloud account) | (cloud account) | Cloud-only auth |
| TP-Link Tapo | TP-Link | All | (cloud account) | (cloud account) | Cloud-only auth |
| Philips Hue Bridge | Philips | All | (button-press auth) | (button-press auth) | Press link button to pair |
| LIFX smart bulb | LIFX | All | (no auth) | (no auth) | Local LAN protocol unauthenticated |
| Mirai/IoT botnet famous defaults | Various | All | mother | fucker | Telnet (in original Mirai list) |
| Mirai/IoT botnet famous defaults | Various | All | tech | tech | Telnet |
| Mirai/IoT botnet famous defaults | Various | All | ubnt | ubnt | SSH |
| Mirai/IoT botnet famous defaults | Various | All | 888888 | 888888 | Telnet |
| Mirai/IoT botnet famous defaults | Various | All | 666666 | 666666 | Telnet |
| Mirai/IoT botnet famous defaults | Various | All | administrator | 1234 | Telnet |
| Mirai/IoT botnet famous defaults | Various | All | admin | 1234 | Telnet |
| Mirai/IoT botnet famous defaults | Various | All | guest | guest | Telnet |
| Mirai/IoT botnet famous defaults | Various | All | admin | 1111 | Telnet |
| Mirai/IoT botnet famous defaults | Various | All | admin | smcadmin | Telnet |
| Mirai/IoT botnet famous defaults | Various | All | root | root | Telnet |
| Mirai/IoT botnet famous defaults | Various | All | admin | password | Telnet/web |
| Mirai/IoT botnet famous defaults | Various | All | root | (blank) | Telnet |
| Mirai/IoT botnet famous defaults | Various | All | support | support | Telnet |
| Mirai/IoT botnet famous defaults | Various | All | root | 54321 | Telnet |
| Mirai/IoT botnet famous defaults | Various | All | root | 123456 | Telnet |
| Mirai/IoT botnet famous defaults | Various | All | root | juantech | Telnet |
| Mirai/IoT botnet famous defaults | Various | All | root | default | Telnet |
| Mirai/IoT botnet famous defaults | Various | All | root | xmhdipc | Telnet (XiongMai) |
| Mirai/IoT botnet famous defaults | Various | All | root | 888888 | Telnet (CCTV chipsets) |
| Mirai/IoT botnet famous defaults | Various | All | root | vizxv | Telnet (Dahua-like) |
| Mirai/IoT botnet famous defaults | Various | All | root | xc3511 | Telnet (XiongMai chipsets) |

## 13. PBX / VoIP

| Product | Vendor | Version(s) | Username | Password | Notes |
|---|---|---|---|---|---|
| Cisco SPA phone | Cisco | All | admin | (blank) | Web admin |
| ShoreTel Director | ShoreTel | All | admin | ShoreTel | Web admin |
| Aastra/Mitel phone web | Aastra | All | admin | 22222 | Web admin |
| Snom phone web | Snom | All | admin | 0000 | Web admin |
| Avaya IP Office | Avaya | All | Operator | Operator | Manager app |
| Avaya IP Office Manager | Avaya | All | Administrator | Administrator | Manager app |
| Asterisk ARI | Digium | All | asterisk | asterisk | REST interface |
| Asterisk Manager (AMI) | Digium | All | admin | amp111 | AMI port 5038 (FreePBX default) |
| FreePBX | Sangoma | All | admin | admin | Web admin |
| 3CX Phone System | 3CX | All | admin | admin | Web admin |
| Cisco Unified CM CLI | Cisco | All | admin | (set on install) | OS admin |
| Cisco Call Manager / CUCM | Cisco | All | ccmadministrator | (set on install) | Web admin |
| Avaya | Avaya | All | (blank) | Craftr4 | From SecLists/cirt.net archive |
| Avaya | Avaya | All | <N/A> | (blank) | From SecLists/cirt.net archive |
| Avaya | Avaya | All | <N/A> | admin | From SecLists/cirt.net archive |
| Avaya | Avaya | All | Administrator | ggdaseuaimhrke | From SecLists/cirt.net archive |
| Avaya | Avaya | All | Craft | crftpw | From SecLists/cirt.net archive |
| Avaya | Avaya | All | admin | admin | https://downloads.avaya.com/css/P8/documents/100173462 |
| Avaya | Avaya | All | admin | admin123 | From SecLists/cirt.net archive |
| Avaya | Avaya | All | admin | barney | From SecLists/cirt.net archive |
| Avaya | Avaya | All | admin | password | https://downloads.avaya.com/css/P8/documents/100181785 |
| Avaya | Avaya | All | craft | (blank) | From SecLists/cirt.net archive |
| Avaya | Avaya | All | dadmin | dadmin | From SecLists/cirt.net archive |
| Avaya | Avaya | All | dadmin | dadmin01 | From SecLists/cirt.net archive |
| Avaya | Avaya | All | diag | danger | From SecLists/cirt.net archive |
| Avaya | Avaya | All | manuf | xxyyzz | From SecLists/cirt.net archive |
| Avaya | Avaya | All | root | ROOT500 | From SecLists/cirt.net archive |
| Avaya | Avaya | All | root | cms500 | From SecLists/cirt.net archive |
| Avaya | Avaya | All | root | ggdaseuaimhrke | From SecLists/cirt.net archive |
| Avaya | Avaya | All | root | root | From SecLists/cirt.net archive |
| GrandStream | GrandStream | All | (blank) | admin | From SecLists/cirt.net archive |
| GrandStream | GrandStream | All | Administrator | admin | From SecLists/cirt.net archive |
| GrandStream | GrandStream | All | End User | 123 (or blank) | From SecLists/cirt.net archive |
| Grandstream Networks, Inc | Grandstream Networks, Inc | All | End User | 123 | http://www.grandstream.com/user_manuals/HandyTone-486UserManual.pdf |
| Grandstream Networks, Inc | Grandstream Networks, Inc | All | admin | admin | http://www.grandstream.com/user_manuals/HandyTone-486UserManual.pdf |
| Grandstream | Grandstream | All | admin | 1234 | From SecLists/cirt.net archive |
| Mitel | Mitel | All | <N/A> | (blank) | From SecLists/cirt.net archive |
| Mitel Networks | Mitel Networks | All | 1nstaller | 5X2000 | http://www.tek-tips.com/viewthread.cfm?qid=1036643 |
| Mitel Networks | Mitel Networks | All | installer | sx2000 | http://www.tek-tips.com/viewthread.cfm?qid=1036643 |
| Mitel Networks | Mitel Networks | All | maint1 | sx2000 | http://www.tek-tips.com/viewthread.cfm?qid=1036643 |
| Mitel Networks | Mitel Networks | All | maint2 | sx2000 | http://www.tek-tips.com/viewthread.cfm?qid=1036643 |
| Mitel Networks | Mitel Networks | All | s1stem | 5X2000 | http://www.tek-tips.com/viewthread.cfm?qid=1036643 |
| Mitel Networks | Mitel Networks | All | system | sx2000 | http://www.tek-tips.com/viewthread.cfm?qid=1036643 |
| Mitel | Mitel | All | installer | 1000 | From SecLists/cirt.net archive |
| Mitel | Mitel | All | system | mnet | From SecLists/cirt.net archive |
| Mitel | Mitel | All | system | password | From SecLists/cirt.net archive |
| Polycom | Polycom | All | (blank) | (blank) | From SecLists/cirt.net archive |
| Polycom | Polycom | All | (blank) | ACCORD | http://www.polycom.com/common/pw_cmp_updateDocKeywords/0,1687,6312,00.pdf |
| Polycom | Polycom | All | (blank) | admin | From SecLists/cirt.net archive |
| Polycom | Polycom | All | (blank) | x6zynd56 | From SecLists/cirt.net archive |
| Polycom | Polycom | All | Polycom | 456 | username is case sensitive |
| Polycom | Polycom | All | Polycom | SpIp | From SecLists/cirt.net archive |
| Polycom | Polycom | All | administrator | * * # | From SecLists/cirt.net archive |
| ShoreTel | ShoreTel | All | Admin | admin1 | From SecLists/cirt.net archive |
| Shoretel | Shoretel | All | admin | changeme | From SecLists/cirt.net archive |
| Snom | Snom | All | Administrator | 0000 | From SecLists/cirt.net archive |
| Aastra | Aastra | All | admin | 33aastra | From SecLists/cirt.net archive |
| Asterisk | Asterisk | All | Admin | admin | From SecLists/cirt.net archive |
| Avaya | Avaya | All | (blank) | admin | From SecLists/cirt.net archive |
| Avaya | Avaya | All | (blank) | (blank) | From SecLists/cirt.net archive |
| Avaya Contact Center (web) | Avaya Contact Center (web) | All | webadmin | webadmin | From SecLists/cirt.net archive |
| Grandstream | Grandstream | All | admin | admin | From SecLists/cirt.net archive |
| grandstream (web) | grandstream (web) | All | admin | admin | From SecLists/cirt.net archive |
| Mitel | Mitel | All | (blank) | (blank) | From SecLists/cirt.net archive |
| Polycom VVX 500 (phone) | Polycom VVX 500 (phone) | All | Admin | 456 | From SecLists/cirt.net archive |
| Polycom VVX 500 (phone) | Polycom VVX 500 (phone) | All | User | 123 | From SecLists/cirt.net archive |
| Snom | Snom | All | admi | (blank) | From SecLists/cirt.net archive |
| Yealink | Yealink | All | admin | admin | From SecLists/cirt.net archive |

## 14. Storage / NAS / SAN

| Product | Vendor | Version(s) | Username | Password | Notes |
|---|---|---|---|---|---|
| Buffalo TeraStation | Buffalo | All | admin | password | Web admin |
| Iomega/LenovoEMC NAS | Lenovo | All | admin | (blank) | Web admin |
| Drobo | Drobo | All | (no auth) | (no auth) | Drobo Dashboard discovery |
| TrueNAS / FreeNAS | iXsystems | All | root | (set on install) | Web wizard |
| WD MyCloud | Western Digital | All | admin | (blank) | Web admin |
| Pure Storage FlashArray | Pure | All | pureuser | pureuser | Web/SSH |
| HPE Nimble | HPE | All | admin | admin | Web admin; must change on first login |
| EqualLogic | Dell | All | grpadmin | grpadmin | Web admin |
| Compellent | Dell EMC | All | Admin | (blank) | Web admin |
| Isilon OneFS | Dell EMC | All | root | a | Web/SSH |
| PowerStore | Dell EMC | All | admin | (set on install) | Web wizard |
| Unisphere / Navisphere | Dell EMC | All | admin | Password123# | Web admin |
| NetApp diag | NetApp | All | diag | (set on install) | Diag mode |
| ONTAP / FilerView | NetApp | All | admin | (set on install) | Web/SSH |
| QTS | QNAP | All | admin | admin | Web admin; must change on first login (newer) |
| DSM legacy | Synology | <6 | admin | (blank) | Older default |
| DSM (DiskStation Manager) | Synology | All | admin | (set on install) | Web wizard |
| EMC | EMC | All | MCUser | MCUser1 | https://community.emc.com/message/525389 |
| EMC | EMC | All | admin | (blank) | EMC Fiber Switch |
| EMC | EMC | All | admin | changeme | https://community.emc.com/message/525389 |
| EMC | EMC | All | backuponly | backuponly1 | https://community.emc.com/message/525389 |
| EMC | EMC | All | backuprestore | backuprestore1 | https://community.emc.com/message/525389 |
| EMC | EMC | All | dpn | changeme | https://community.emc.com/message/525389 |
| EMC | EMC | All | restoreonly | restoreonly1 | https://community.emc.com/message/525389 |
| EMC | EMC | All | root | 8RttoTriz | https://community.emc.com/message/525389 |
| EMC | EMC | All | root | changeme | https://community.emc.com/message/525389 |
| EMC | EMC | All | viewuser | viewuser1 | https://community.emc.com/message/525389 |
| NetApp | NetApp | All | admin | NetCache | From SecLists/cirt.net archive |
| NetApp | NetApp | All | admin | admin123 | From SecLists/cirt.net archive |
| Nimble | Nimble | All | (blank) | xdfk9874t3 | From SecLists/cirt.net archive |
| Nimble | Nimble | All | <N/A> | xdfk9874t3 | From SecLists/cirt.net archive |
| Synology Inc | Synology Inc | All | admin | (blank) | http://forum.synology.com/wiki/index.php/Quick_Install_Guide:_Installing_the_Synology_Server |
| FreeNAS (web) | FreeNAS (web) | All | root | freenas | From SecLists/cirt.net archive |
| NetApp ONTAP | NetApp ONTAP | All | admin | netapp!123 | From SecLists/cirt.net archive |
| NetApp ONTAP System Manager | NetApp ONTAP System Manager | All | admin | admin123 | From SecLists/cirt.net archive |
| QNAP (QTS/QuTS hero 4.4.1 - 4.3.6 or earlier) | QNAP (QTS/QuTS hero 4.4.1 - 4.3.6 or earlier) | All | admin | admin | From SecLists/cirt.net archive |
| QNAP (QTS/QuTS hero 4.4.2 - 5.1.x) | QNAP (QTS/QuTS hero 4.4.2 - 5.1.x) | All | admin | 1st MAC address of NAS (uppercase letters without special characters) [ex: MAC = 00-08-9B-F6-15-75 / password = 00089BF61575] | From SecLists/cirt.net archive |
| QNAP (QTS/QuTS hero 5.2.0 and later (5.2.x 5.3.x 6.0.0)) | QNAP (QTS/QuTS hero 5.2.0 and later (5.2.x 5.3.x 6.0.0)) | All | admin | Cloud Key of NAS (uppercase letters without any special characters) [ex: Cloud Key = Q1234-5678 / password = Q12345678] | From SecLists/cirt.net archive |
| QNAP QTS (web) | QNAP QTS (web) | All | admin | admin | From SecLists/cirt.net archive |
| Synology DSM (web) | Synology DSM (web) | All | admin | (blank) | From SecLists/cirt.net archive |

## 15. Backup software

| Product | Vendor | Version(s) | Username | Password | Notes |
|---|---|---|---|---|---|
| Bacula Director | Bacula | All | (config-file password) | (config-file password) | BAT/bconsole |
| Unitrends | Unitrends | All | admin | (set on install) | Web admin |
| Unitrends | Unitrends | All | root | unitrends1 | SSH |
| Arcserve UDP | Arcserve | All | (set on install) | (set on install) | Web wizard |
| Acronis Cyber Protect | Acronis | All | (set on install) | (set on install) | Web wizard |
| Veritas NetBackup | Veritas | All | (OS account) | (OS account) | Uses host OS auth |
| Cohesity DataProtect | Cohesity | All | admin | admin | Web admin; must change on first login |
| Rubrik CDM | Rubrik | All | admin | (set on install) | Web wizard |
| Commvault CommServe | Commvault | All | admin | (set on install) | Web admin |
| Veeam Enterprise Manager | Veeam | All | admin | (set on install) | Web admin |
| Veeam Backup & Replication | Veeam | All | (uses Windows account) | (uses Windows account) | Console; no separate default |
| Veritas | Veritas | All | admin | password | From SecLists/cirt.net archive |
| NetBackup OpsCenter Analytics (web) | NetBackup OpsCenter Analytics (web) | All | admin | password | From SecLists/cirt.net archive |

## 16. Identity / auth

| Product | Vendor | Version(s) | Username | Password | Notes |
|---|---|---|---|---|---|
| Shibboleth IdP | Shibboleth | All | (no admin UI) | (no admin UI) | File-config only |
| RSA Authentication Manager | RSA | All | admin | (set on install) | Web admin |
| Cisco ACS | Cisco | All | acsadmin | default | Web admin |
| Cisco ISE | Cisco | All | admin | (set on install) | Web/SSH |
| Keycloak | Red Hat | All | admin | admin | Common dev install; production wizard |
| FreeIPA | Red Hat | All | admin | (set on ipa-server-install) | Web/Kerberos |
| LDAP common dev | OpenLDAP | All | cn=admin,dc=example,dc=com | (set on slapadd) | rootDN; common dev |
| Active Directory built-in | Microsoft | All | krbtgt | (random, rotated) | Service account |
| Active Directory built-in | Microsoft | All | Guest | (disabled) | Built-in; disabled by default |
| Active Directory | Microsoft | All | Administrator | (set on promo) | Built-in; password set during dcpromo |
| daloradius | daloradius | All | administrator | radius | From SecLists/cirt.net archive |
| keycloak | keycloak | All | keycloak-admin | datical | From SecLists/cirt.net archive |
| ldap account manager(lam) | ldap account manager(lam) | All | lam | lam | From SecLists/cirt.net archive |

## 17. Containers / orchestrators

| Product | Vendor | Version(s) | Username | Password | Notes |
|---|---|---|---|---|---|
| Vault | HashiCorp | All | (generated init token) | (generated init token) | vault operator init |
| Consul | HashiCorp | All | (no ACL) | (no ACL) | Default has no ACL |
| etcd | CoreOS | All | (no auth) | (no auth) | Default has no auth |
| MicroK8s | Canonical | All | (token-based) | (token-based) | Use microk8s config |
| Minikube dashboard | Kubernetes | All | (no auth) | (no auth) | Local only |
| Docker Registry v2 | Docker | All | (no auth) | (no auth) | Default has no auth; htpasswd optional |
| OpenShift | Red Hat | All | kubeadmin | (generated, in auth/kubeadmin-password) | Web/CLI |
| Kubernetes Dashboard | Kubernetes | All | (token-based) | (token-based) | ServiceAccount token |
| Portainer | Portainer | All | admin | (set on first login, must be 12+ chars) | Web admin |
| Rancher | SUSE/Rancher | <2.6 | admin | admin | Web admin |
| Rancher | SUSE/Rancher | >=2.6 | admin | (generated, run rancher to view) | Web admin |

## 18. SaaS-style appliances

| Product | Vendor | Version(s) | Username | Password | Notes |
|---|---|---|---|---|---|
| Imperva SecureSphere | Imperva | All | admin | admin | Web admin |
| Cisco FTD/FMC | Cisco | All | admin | Admin123 | Web; must change on first login |
| Cisco ASA / FTD | Cisco | All | (blank) | (blank) | Console; enable secret unset |
| Pulse Secure / Ivanti CS | Ivanti | All | admin | (set on install) | Web wizard |
| NetScaler/Citrix ADC (newer) | Citrix | >=12.1 build 49 | nsroot | (serial number) | Must use serial as initial password |
| NetScaler/Citrix ADC | Citrix | All | nsroot | nsroot | Web/SSH |
| F5 BIG-IP CLI | F5 | All | root | default | SSH |
| F5 BIG-IP | F5 | All | admin | admin | Web; must change on first login |
| Sophos XG/Firewall | Sophos | All | admin | admin | Web admin; must change on first login |
| Sophos UTM/SG | Sophos | All | loginuser | (set on install) | Web admin |
| Splunk Enterprise | Splunk | <7.1 | admin | changeme | Web admin |
| Barracuda | Barracuda | All | admin | admin | http://www.barracudanetworks.com/ns/downloads/Quick_Start_Guides/QSG_Barracuda_SSLVPN_US.pdf |
| Barracuda | Barracuda | All | ssladmin | ssladmin | http://www.barracudanetworks.com/ns/downloads/Quick_Start_Guides/QSG_Barracuda_SSLVPN_US.pdf |
| F5 BIG-IP Configuration utility | F5 BIG-IP Configuration utility | All | admin | admin | https://support.f5.com/csp/article/K13148 |
| F5 BIG-IP command line | F5 BIG-IP command line | All | root | default | https://support.f5.com/csp/article/K13148 |
| Barracuda (web) | Barracuda (web) | All | admin | admin | From SecLists/cirt.net archive |
| Barracuda (web) | Barracuda (web) | All | ssladmin | ssladmin | From SecLists/cirt.net archive |
| Pulse Secure | Pulse Secure | All | admin | password | From SecLists/cirt.net archive |

## 19. Misc dev tools

| Product | Vendor | Version(s) | Username | Password | Notes |
|---|---|---|---|---|---|
| Bonita BPM | Bonitasoft | All | walter.bates | bpm | Tenant admin |
| Bonita BPM | Bonitasoft | All | install | install | Platform admin |
| Metabase | Metabase | All | (set on first run) | (set on first run) | Web wizard |
| Superset | Apache | All | admin | (set via superset fab create-admin) | Web admin |
| Airflow | Apache | >=2 | (set via airflow users create) | (set via airflow users create) | Must run users-create |
| Airflow | Apache | <2 | admin | admin | Web admin |
| RStudio Server | Posit | All | (uses OS account) | (uses OS account) | PAM auth |
| Jupyter Notebook | Jupyter | All | (token-based) | (token-based) | Token printed at startup |
| GitLab default root | GitLab | <14 | root | 5iveL!fe | Web admin |
| Directus | Directus | All | admin@example.com | d1r3ctu5 | Web admin (dev) |
| Strapi | Strapi | All | (set on first run) | (set on first run) | Web wizard |
| ElasticHQ | ElasticHQ | All | (no auth) | (no auth) | Default has no auth |
| Mongo Express | Mongo Express | All | admin | pass | Web admin |
| Kafka Manager (CMAK) | Yahoo | All | (no auth) | (no auth) | Default has no auth |
| RabbitMQ Management | RabbitMQ | All | guest | guest | Web admin (localhost-only by default) |
| phpPgAdmin | phpPgAdmin | All | (uses postgres creds) | (uses postgres creds) | Login uses postgres |
| Adminer | Adminer | All | (uses DB creds) | (uses DB creds) | Login uses underlying DB |
| Jenkins (post-wizard) | Jenkins | All | admin | admin | Web admin |
| Tomcat Manager | Apache | All | tomcat | tomcat | Web manager |
| Redmine | Redmine | All | admin | admin | From SecLists/cirt.net archive |

## Sources

- SecLists `Passwords/Default-Credentials/` — https://github.com/danielmiessler/SecLists/tree/master/Passwords/Default-Credentials
- SecLists `default-passwords.csv` — https://raw.githubusercontent.com/danielmiessler/SecLists/master/Passwords/Default-Credentials/default-passwords.csv
- ihebski `DefaultCreds-cheat-sheet` — https://github.com/ihebski/DefaultCreds-cheat-sheet
- cirt.net default password database — https://cirt.net/passwords
- DefaultPassword.us archive — https://default-password.info/
- RouterPasswords.com — https://www.routerpasswords.com/
- HP iLO / iDRAC / IPMI vendor admin guides
- Hikvision CVE-2017-7921 advisory — https://nvd.nist.gov/vuln/detail/CVE-2017-7921
- Mirai botnet original credential list (Krebs on Security 2016) — https://krebsonsecurity.com/2016/10/who-makes-the-iot-things-under-attack/
- Vendor product manuals (Cisco/Juniper/Fortinet/Palo Alto/MikroTik/Ubiquiti/Aruba/Sophos/SonicWall/etc.)
- Wonderware/AVEVA, Siemens SIMATIC, Rockwell, Schneider, Mitsubishi, Tridium Niagara product documentation
- Synology/QNAP/NetApp/Dell EMC/HPE Nimble/Pure Storage admin guides
- Splunk/Grafana/Kibana/SonarQube/Nexus/Artifactory/Harbor/ArgoCD official docs
- Atlassian/Bitnami/WordPress/Drupal/Joomla install documentation
