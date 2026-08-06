# Backup & Disaster Recovery

## Overview

Design and operation of backup and disaster recovery strategies covering physical and virtual workloads, endpoint devices, and configuration data. Includes hypervisor-level backup, NAS-based storage, encrypted cloud backup, retention policy design, and validated restore procedures.

## Technologies & tools

- **Veeam** — primary enterprise backup platform, both hypervisor-level and endpoint
- **Proxmox VE** — full hypervisor backup and migration on physical servers
- **QNAP** — primary NAS storage for backup targets
- **Microsoft Azure Backup** — off-site cloud backup for selected workloads
- **NinjaOne** — cloud encrypted backup for endpoints managed via RMM

## Responsibilities & operational scope

- Backup strategy design including storage tiering and disaster recovery planning
- Full hypervisor-level backup and migration of Proxmox VE on physical servers
- Configuration of backup/restore jobs, tuning, capacity planning, and problem resolution
- Backup policy management: tuning, capacity planning, restore procedures and retention windows
- Archiving and long-term retention of data and configuration snapshots
- Ensuring IT governance procedures around backup and recovery are documented and kept up to date

## Known interoperability issues tracked

- Windows 11 24H2 compatibility with Veeam Agent — internal procedures aligned with vendor KB guidance

## Projects & evidence

### Avoid Microsoft account during Win11 setup
<!-- graphify-evidence-id: b3d28403307c -->

- **Source**: `0. Per evitare l'accesso con account Microsoft.txt`

*Evidence text to be enriched from source document.*

*Technology stack: to be enriched from source document.*

### Piano 1 - Ufficio IT
<!-- graphify-evidence-id: 711eaef61765 -->

- **Source**: `ARCHITETTURA [HOSTNAME_56] 20052026_b5a58014.md`
- **Graph community**: 0

Dal Cisco c’è attaccato l’adattatore PoE che poi è connesso alla 0.7.1 come AP mentre l’ultima terza porta del Cisco è diretta alla 0-R-18. Poi c'è un concentratore rete per visualizzare i parametri d

*Technology stack: to be enriched from source document.*

### Piano 2 - Rack DX (Armadio server)
<!-- graphify-evidence-id: 91c1b768e4cf -->

- **Source**: `ARCHITETTURA [HOSTNAME_56] 20052026_b5a58014.md`
- **Graph community**: 0

Considerando che [RIMOSSO] non è attivo e [RIMOSSO] nemmeno e che G9 è stato spento in data 19/12/2024. Sbagliato, da correggere l’ordine Inoltre, riprendendo le informazioni del paragrafo Concetti gen

*Technology stack: to be enriched from source document.*

### HP ProLiant DL380 Gen 10 (host Proxmox)
<!-- graphify-evidence-id: b97531aa4380 -->

- **Source**: `ARCHITETTURA [HOSTNAME_56] 20052026_b5a58014.md`
- **Graph community**: 0

A partire da due settimane dopo il subentro della nuova linea dati FTTO Vianova. In data 20/01/2025 è arrivato un tecnico della TIM che ha fatto un sopralluogo per ampliare l’infrastruttura hardware (

*Technology stack: to be enriched from source document.*

### HP ProLiant DL360 G9 (spento 19/12/2024)
<!-- graphify-evidence-id: a0eec3ccaa1c -->

- **Source**: `ARCHITETTURA [HOSTNAME_56] 20052026_b5a58014.md`
- **Graph community**: 0

(per creare VM ecc.) | | SEEWEB - Foundation Server PRO - Tivoli Backup | https://[RIMOSSO]/signin | [EMAIL_29] | oQui0uhu | 26/05/2021 | | | Funzione | Gestione da N

*Technology stack: to be enriched from source document.*

### Proxmox Virtual Environment 8.3.4
<!-- graphify-evidence-id: 45223e306d2f -->

- **Source**: `ARCHITETTURA [HOSTNAME_56] 20052026_b5a58014.md`
- **Graph community**: 0

Che include appunto Proxmox Virtual Environment versione open source e la CREAZIONE E INSTALLAZIONE 2 VM LINUX e 1 VM Windows SERVER 2022. In data 28/01 come da conversazione con [PERSONA_2] (privata

*Technology stack: to be enriched from source document.*

### HP iLO5 (interfaccia gestione HP)
<!-- graphify-evidence-id: 3a77df047a3a -->

- **Source**: `ARCHITETTURA [HOSTNAME_56] 20052026_b5a58014.md`
- **Graph community**: 0

La tabella della mail è stata aggiornata considerando il dettaglio nel preventivo. L’idea sarebbe di andare sul ricondizionato, è il modello precedente, ma di fascia molto più alta. L’alternativa è fa

*Technology stack: to be enriched from source document.*

### VM Ubuntu 10.10 Svn ([IP_10])
<!-- graphify-evidence-id: 48839b31a978 -->

- **Source**: `ARCHITETTURA [HOSTNAME_56] 20052026_b5a58014.md`
- **Graph community**: 0

C’è una differenza tra "Virtual Server", "1:1 NAT" e "Many 1:1 NAT" nella sezione NAT > Classification dello Zyxel che può creare confusione. In pratica: - Virtual Server: è quando si vogliono mappare

*Technology stack: to be enriched from source document.*

### VM Ubuntu 10.10 TestWeb ([IP_22], Mantis)
<!-- graphify-evidence-id: a52d634c39a1 -->

- **Source**: `ARCHITETTURA [HOSTNAME_56] 20052026_b5a58014.md`
- **Graph community**: 0

- WebTest - (nome VM: Ubuntu 10.10 TestWeb) - UBUNTU-WEBTEST - Sopra a questo c’è Mantis per i ticket interni - Accesso via “ssh” - IP:[IP_22] (IP pubblico: [IP_49]) - Php per test - IP:19

*Technology stack: to be enriched from source document.*

### [HOSTNAME_6] Linux (nuova, su Proxmox)
<!-- graphify-evidence-id: 41c519669d20 -->

- **Source**: `ARCHITETTURA [HOSTNAME_56] 20052026_b5a58014.md`
- **Graph community**: 0

Quindi, la password macchina Virtual Machine 101 ([HOSTNAME_5]) on node ‘pve’ (Windows): Administrator emmapo3011(pse) Password macchina Virtual Machine 100 ([HOSTNAME_6]) on node ‘pve’ (Linux): - Prova - 1234 Qui

*Technology stack: to be enriched from source document.*

### Mantis (ticketing interno)
<!-- graphify-evidence-id: fbef18aad6eb -->

- **Source**: `ARCHITETTURA [HOSTNAME_56] 20052026_b5a58014.md`
- **Graph community**: 0

Ora la scheda di rete è correttamente configurata. L'altra macchina Ubuntu 10.10 TestWeb ([IP_22] – Servizio ticketing interno Mantis) invece funzionava in automatico: Così come: La macchina Ub

*Technology stack: to be enriched from source document.*

### MKSBackup (con ghettoVCB)
<!-- graphify-evidence-id: 5e63a2df09d1 -->

- **Source**: `ARCHITETTURA [HOSTNAME_56] 20052026_b5a58014.md`
- **Graph community**: 0

- Le configurazioni dei backup si trovano nel file /etc/mksbackup/mksbackup.ini su [IP_10], (nel file /etc/mksbackup/vmware/ghettoVCB.conf invece ci sono configurazioni più generiche e sul mod

*Technology stack: to be enriched from source document.*

### Veeam Backup Agent (postazioni di lavoro)
<!-- graphify-evidence-id: a8c5ce4550f5 -->

- **Source**: `ARCHITETTURA [HOSTNAME_56] 20052026_b5a58014.md`
- **Graph community**: 0

Per eliminare tutta la cartella (processo che impiega tempo dato che gli HD del NAS sonovecchi e lenti in lettura e/o scrittura). Backup postazioni di lavoro (con Veeam) Come step successivo si vu

*Technology stack: to be enriched from source document.*

### myQNAPcloud Storage (backup cloud)
<!-- graphify-evidence-id: 7b97c4df20ac -->

- **Source**: `ARCHITETTURA [HOSTNAME_56] 20052026_b5a58014.md`
- **Graph community**: 11

Inoltre, a livello di funzionalità software si può considerare: - RAID supportati: JBOD, RAID 0, RAID 1 - Servizi di rete: CIFS/SMB, AFP, NFS, FTP, HTTP/HTTPS, iSCSI, DLNA, UPnP - Backup: Supporto per

*Technology stack: to be enriched from source document.*

### Microsoft Azure Backup (in dismissione)
<!-- graphify-evidence-id: eaf28490dd2f -->

- **Source**: `ARCHITETTURA [HOSTNAME_56] 20052026_b5a58014.md`
- **Graph community**: 11

La tabella della mail è stata aggiornata considerando il dettaglio nel preventivo. L’idea sarebbe di andare sul ricondizionato, è il modello precedente, ma di fascia molto più alta. L’alternativa è fa

*Technology stack: to be enriched from source document.*

### Configurazione RAID 1 (mirror)
<!-- graphify-evidence-id: cc84660b2e10 -->

- **Source**: `ARCHITETTURA [HOSTNAME_56] 20052026_b5a58014.md`
- **Graph community**: 0

Questo significa che i dischi sono configurati (alla data del 27/06/2025) in RAID 1 (Mirroring) cioè: - I dati scritti su un disco vengono copiati identicamente sull’altro. - Se uno dei due dischi si

*Technology stack: to be enriched from source document.*

### Flusso backup VM (Proxmox verso NAS)
<!-- graphify-evidence-id: 9e5a11d16a3a -->

- **Source**: `ARCHITETTURA [HOSTNAME_56] 20052026_b5a58014.md`

*Evidence text to be enriched from source document.*

*Technology stack: to be enriched from source document.*

### Backup TM Groupshare automatizzato
<!-- graphify-evidence-id: 516f93618b6c -->

- **Source**: `ARCHITETTURA [HOSTNAME_56] 20052026_b5a58014.md`

*Evidence text to be enriched from source document.*

*Technology stack: to be enriched from source document.*

### Create Restore Point.ps1
<!-- graphify-evidence-id: ec03ae5e579c -->

- **Source**: `Create Restore Point.ps1`
- **Graph community**: 31

Function to create restore point with progress reporting function Create-RestorePoint { Write-Host "Starting to create restore point..." -ForegroundColor Yellow Simulate progress for ($i =

*Technology stack: to be enriched from source document.*

### Create-RestorePoint()
<!-- graphify-evidence-id: b88824e7ae57 -->

- **Source**: `Create Restore Point.ps1`
- **Graph community**: 31

Function to create restore point with progress reporting function Create-RestorePoint { Write-Host "Starting to create restore point..." -ForegroundColor Yellow Simulate progress for ($i =

*Technology stack: to be enriched from source document.*

### Restore all built-in apps.ps1
<!-- graphify-evidence-id: 58f0dcf88a91 -->

- **Source**: `Restore all built-in apps.ps1`
- **Graph community**: 44

if (-not ([Security.Principal.WindowsPrincipal][Security.Principal.WindowsIdentity]::GetCurrent()).IsInRole([Security.Principal.WindowsBuiltInRole]::Administrator)) { Write-Warning "This script mu

*Technology stack: to be enriched from source document.*

### Create Restore Point.ps1
<!-- graphify-evidence-id: 0581e6bc5d6f -->

- **Source**: `Create Restore Point.ps1`
- **Graph community**: 50

﻿# Create a system restore point (safety net before changes) Host: console Category: Tool Options: Create restore point param([string]$choice) if ($choice -eq "Create restore point") { Che

*Technology stack: to be enriched from source document.*

### Microsoft Defender maintenance.ps1
<!-- graphify-evidence-id: 7e84d780f508 -->

- **Source**: `Microsoft Defender maintenance.ps1`
- **Graph community**: 19

﻿# Microsoft Defender maintenance (update signatures, repair, show status) Category: Tool Options: Update signatures; Repair definitions and update (console); Show Defender status (console) param(

*Technology stack: to be enriched from source document.*

### Get-MpCmdPath()
<!-- graphify-evidence-id: 8a1d4dc72c08 -->

- **Source**: `Microsoft Defender maintenance.ps1`
- **Graph community**: 19

function Get-MpCmdPath { $candidates = @( "$env:ProgramFiles\Windows Defender\MpCmdRun.exe", "$env:ProgramFiles\Microsoft Defender\MpCmdRun.exe" ) foreach ($p in $candidate

*Technology stack: to be enriched from source document.*

### Show-Status()
<!-- graphify-evidence-id: e2f916662b61 -->

- **Source**: `Microsoft Defender maintenance.ps1`
- **Graph community**: 19

﻿# Microsoft Defender maintenance (update signatures, repair, show status) Category: Tool Options: Update signatures; Repair definitions and update (console); Show Defender status (console) param(

*Technology stack: to be enriched from source document.*

### Restore all built-in apps.ps1
<!-- graphify-evidence-id: 25e8d02e5e7e -->

- **Source**: `Restore all built-in apps.ps1`
- **Graph community**: 56

if (-not ([Security.Principal.WindowsPrincipal][Security.Principal.WindowsIdentity]::GetCurrent()).IsInRole([Security.Principal.WindowsBuiltInRole]::Administrator)) { Write-Warning "This script mu

*Technology stack: to be enriched from source document.*

### Migrazione Authenticator via backup cloud
<!-- graphify-evidence-id: 450d4bca3f77 -->

- **Source**: `Authenticator e Entra ID.txt`
- **Graph community**: 4

L’immagine mostra una schermata in cui viene richiesto il codice generato da Microsoft Authenticator, ma sul dispositivo nuovo non appare alcun account configurato. Questo scenario, unito all’errore 5

*Technology stack: to be enriched from source document.*

### %LOCALAPPDATA%\Programs\Microsoft VS Code (installazione)
<!-- graphify-evidence-id: da55101ea248 -->

- **Source**: `Perche inoltre ho tre cartelle di i.txt`
- **Graph community**: 20

*Evidence text to be enriched from source document.*

*Technology stack: to be enriched from source document.*

### System Repair & Recovery Flow
<!-- graphify-evidence-id: 86b5284207cc -->

- **Source**: `scripts`

*Evidence text to be enriched from source document.*

*Technology stack: to be enriched from source document.*

### LAN Intrawelt [IP_89] (server)
<!-- graphify-evidence-id: 6eb205b7355d -->

- **Source**: `ARCHITETTURA [HOSTNAME_56] 20052026_b5a58014.md`
- **Graph community**: 0

I file da prendere in considerazione sono questi tre: - Architettura Server Intrawelt-punto-informatica.ppt - Queste informazioni sono state ampliate e messe in maniera ordinata nei successivi paragra

*Technology stack: to be enriched from source document.*

### Punto Informatica (fornitore IT)
<!-- graphify-evidence-id: 6ba1148b7b4b -->

- **Source**: `ARCHITETTURA [HOSTNAME_56] 20052026_b5a58014.md`
- **Graph community**: 0

Alla piattaforma di monitoraggio e gestione avranno accesso sia i tecnici IT del fornitore che quelli del cliente. Al punto 5.7 specifica che il cliente può richiedere supporto tecnico per qualunque t

*Technology stack: to be enriched from source document.*
