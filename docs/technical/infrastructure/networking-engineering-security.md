# Networking Engineering & Security

## Overview

Design and operation of structured corporate networks spanning LAN, WAN, Wi-Fi, VPN, and segmented VLAN topologies, with physical and cloud-based firewall enforcement. Covers identity-based access, bandwidth management, endpoint detection and response integration, and domain/DNS lifecycle operations.

## Technologies & tools

- **IPsec VPN** — internal and external remote access
- **Bitdefender GravityZone** — EDR platform
- **WordPress** admin — for hosted/CMS workloads
- **Aruba**, **Fastnet** — domain registration and hosting providers
- Physical and cloud-based firewall systems (vendor-agnostic experience)

## Responsibilities & operational scope

- Networking concepts and DHCP administration
- Network and server monitoring with anomaly detection and resolution
- Network security policy enforcement
- LAN access management for internal and external users via IPsec VPN, with network segmentation
- Design of structured networks: WAN, LAN, Wi-Fi, VPN, VLAN restrictions, physical and cloud firewall systems
- Firewall implementation, management, and customization
- VPN configuration and secure remote access provisioning
- Security incident monitoring and response
- EDR management (Bitdefender GravityZone) including policy deployment
- Network bandwidth allocation and QoS policies
- Domain lifecycle expertise: CMS administration, redirects, registration, hosting migration and backup (WordPress, Aruba, Fastnet)

## Projects & evidence

### ZYXEL USG FLEX 500 (Firewall/VPN)
<!-- graphify-evidence-id: 7857744caa40 -->

- **Source**: `ARCHITETTURA [HOSTNAME_56] 20052026_b5a58014.md`
- **Graph community**: 2

Quindi sulla porta 52 dello Zyxel [HOSTNAME_59] al piano 2 arriva una connessione configurata come uplink con capacità potenziale di 10 gigabit al secondo. L’indicazione Speed 10G/Auto (SFP+) significa

*Technology stack: to be enriched from source document.*

### Supremo Remote Control (alternativa VPN)
<!-- graphify-evidence-id: f5e397a0685c -->

- **Source**: `ARCHITETTURA [HOSTNAME_56] 20052026_b5a58014.md`
- **Graph community**: 2

Le timbrature staranno su un database SQL da poter esportare su un’altra macchina o su un database interno. Vedere chiamando loro se BioStar ha una procedura di esportazione > importazione. - Installa

*Technology stack: to be enriched from source document.*

### Aruba (hosting/DNS domini)
<!-- graphify-evidence-id: 33508ef0e796 -->

- **Source**: `ARCHITETTURA [HOSTNAME_56] 20052026_b5a58014.md`
- **Graph community**: 5

SITI WEB E DOMINI Il caso [RIMOSSO] In data 20/01/2025 alle 15:39 [PERSONA_4] manda una mail dicendo che quasi per caso ha controllato la posta che arriva relativa a SAB e ha notato che ent

*Technology stack: to be enriched from source document.*

### Intrawelt Policy VPN
<!-- graphify-evidence-id: d06e8b09b50b -->

- **Source**: `problema connessione RDP LAN.md`
- **Graph community**: 0

vedere Intrawelt Policy VPN Il firewall è spento provo a disattivare del tutto gravity

*Technology stack: to be enriched from source document.*

### Fastnet S.p.a. (provider hosting/DNS)
<!-- graphify-evidence-id: fc6ab32ff48b -->

- **Source**: `ARCHITETTURA [HOSTNAME_56] 20052026_b5a58014.md`
- **Graph community**: 5

(…) In particolare: - Name Server: [RIMOSSO], [RIMOSSO]: i i server che gestiscono la traduzione del nome di dominio in indirizzi IP. In questo caso, i server di Fastnet gestiscono il

*Technology stack: to be enriched from source document.*

### Stack VPN client-firewall-seeweb
<!-- graphify-evidence-id: 7cab29c274e8 -->

- **Source**: `ARCHITETTURA [HOSTNAME_56] 20052026_b5a58014.md`

*Evidence text to be enriched from source document.*

*Technology stack: to be enriched from source document.*

### Accesso remoto aziendale (VPN + RDP + telefono IP su PC)
<!-- graphify-evidence-id: 8c58d11a2c2f -->

- **Source**: `shared`

*Evidence text to be enriched from source document.*

*Technology stack: to be enriched from source document.*

### Gestione firewall ZYXEL (portali cloud + licensing + config policy)
<!-- graphify-evidence-id: 258d9579c34f -->

- **Source**: `shared`

*Evidence text to be enriched from source document.*

*Technology stack: to be enriched from source document.*

### Boot Access Helper.ps1
<!-- graphify-evidence-id: 4d6ee94e25ef -->

- **Source**: `Boot Access Helper.ps1`
- **Graph community**: 14

﻿# Description: Shows common Boot Menu and BIOS/UEFI keys based on detected manufacturer (info-only). Category: Tool Host: embedded Options: Show info dialog; Print to output (log) param( [str

*Technology stack: to be enriched from source document.*

### Get-SystemVendor()
<!-- graphify-evidence-id: 71aaf2fe9f92 -->

- **Source**: `Boot Access Helper.ps1`
- **Graph community**: 14

function Get-SystemVendor { try { $cs = Get-CimInstance -ClassName Win32_ComputerSystem $m = "" $mo = "" if ($cs -and $cs.Manufacturer -ne $null) { $m = [string]$cs.Manufacturer } if (

*Technology stack: to be enriched from source document.*

### Get-VendorMap()
<!-- graphify-evidence-id: fdd250d20c65 -->

- **Source**: `Boot Access Helper.ps1`
- **Graph community**: 14

function Get-VendorMap { Array of hashtables (super compatible) return @( @{ Vendor="Acer"; BootMenu="F12"; BiosSetup="F2" }, @{ Vendor="ASUS"; BootMenu="Esc

*Technology stack: to be enriched from source document.*

### Build-Content()
<!-- graphify-evidence-id: 5ee0d43975d9 -->

- **Source**: `Boot Access Helper.ps1`
- **Graph community**: 14

function Build-Content { $map = Get-VendorMap $sys = Get-SystemVendor $manufacturer = $sys.Manufacturer $model = $sys.Model $sb = New-Object System.Text.StringBuilder [void]$sb.AppendLine("B

*Technology stack: to be enriched from source document.*

### Show-Dialog()
<!-- graphify-evidence-id: 60982fc66781 -->

- **Source**: `Boot Access Helper.ps1`
- **Graph community**: 14

﻿# Description: Shows common Boot Menu and BIOS/UEFI keys based on detected manufacturer (info-only). Category: Tool Host: embedded Options: Show info dialog; Print to output (log) param( [str

*Technology stack: to be enriched from source document.*

### Utente amministratore PC
<!-- graphify-evidence-id: 63c6e391b6e9 -->

- **Source**: `Configurazione-PC-autenticazione.md`
- **Graph community**: 4

Gestione PC Ogni postazione Pc deve avere due utenti presenti: - Un utente amministratore accessibile solo al personale IT - Un utente standard accessibile dagli utenti del pc L'utente standard può ut

*Technology stack: to be enriched from source document.*

### Utente standard PC
<!-- graphify-evidence-id: fbbae382a2a0 -->

- **Source**: `Configurazione-PC-autenticazione.md`
- **Graph community**: 4

Gestione PC Ogni postazione Pc deve avere due utenti presenti: - Un utente amministratore accessibile solo al personale IT - Un utente standard accessibile dagli utenti del pc L'utente standard può ut

*Technology stack: to be enriched from source document.*

### Due utenti per PC (admin IT + standard)
<!-- graphify-evidence-id: 1b7869e2e813 -->

- **Source**: `Configurazione-PC-autenticazione.md`
- **Graph community**: 4

Gestione PC Ogni postazione Pc deve avere due utenti presenti: - Un utente amministratore accessibile solo al personale IT - Un utente standard accessibile dagli utenti del pc L'utente standard può ut

*Technology stack: to be enriched from source document.*

### Firewall aziendale
<!-- graphify-evidence-id: aac0b874755b -->

- **Source**: `Regolamento-utilizzo-strumenti-informatici.md`
- **Graph community**: 7

1. PRINCIPI GENERALI Il presente documento ha l’obiettivo di regolamentare l’accesso alla postazione di lavoro, l’utilizzo del telefono cellulare, di internet e della posta elettronica per gli utent

*Technology stack: to be enriched from source document.*

### Problema connessione RDP LAN
<!-- graphify-evidence-id: 45d992ef193a -->

- **Source**: `problema connessione RDP LAN.md`
- **Graph community**: 0

Lo scopo è quello di permettere a RDP di accettare una connessione che arriva da un hotspot situato in spagna, la connessione alla VPN aziendale invece avviene senza problemi. E poi non fa modificare

*Technology stack: to be enriched from source document.*

### Endpoint exception for Advanced IP Scanner
<!-- graphify-evidence-id: 0845cc5c02be -->

- **Source**: `advancedIPscanner eccezione su [HOSTNAME_1].md`
- **Graph community**: 2

"C:\Program Files (x86)\Advanced IP Scanner\advanced_ip_scanner.exe"

*Technology stack: to be enriched from source document.*

### Bitdefender GravityZone Cloud console
<!-- graphify-evidence-id: fbf7eb35d6ee -->

- **Source**: `Migrazione-ESET-Bitdefender-primo-accesso.md`
- **Graph community**: 0

https://cloudgz.gravityzone.bitdefender.com [PERSONA_9], [09/09/2025 12:47] ho creato account con tua mail, basta che fai il recupero e ti puoi loggare

*Technology stack: to be enriched from source document.*

### Continuous cybersec learning / vendor webinars
<!-- graphify-evidence-id: 1050ec0173ae -->

- **Source**: `on top of cybersec trends.md`
- **Graph community**: 0

https://www.bitdefender.com/en-us/business/webinars?_gl=1*1x4sven*_gcl_au*MTg5OTEwNzc2OC4xNzU3OTI2NDQz*_ga*Nzc3Mzk2NjA4LjE3NTg1NTM4ODA.*_ga_6M0GWNLLWF*czE3NTg1NTM4NzkkbzEkZzEkdDE3NTg1NTQwNzgkajUyJGwwJ

*Technology stack: to be enriched from source document.*

### Endpoint hardening program (exceptions, firewall policy, password protection, 2FA)
<!-- graphify-evidence-id: 0acaa35ed843 -->

- **Source**: `Protezione avanzata (LAN) Intrawelt.md`

*Evidence text to be enriched from source document.*

*Technology stack: to be enriched from source document.*

### Flusso troubleshooting DNS/hostname sui 5 PC problematici
<!-- graphify-evidence-id: 1eae13824507 -->

- **Source**: `flushare cache DNS da cmd.md`

*Evidence text to be enriched from source document.*

*Technology stack: to be enriched from source document.*
