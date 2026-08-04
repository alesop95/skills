# System Administration

## Overview

Formal system administrator role with end-to-end responsibility for
physical and virtual server fleet, endpoint estate, and centralized
remote monitoring. Covers Windows and Linux/Unix administration, RMM-
driven operations, certificate and secure-communication management, and
custom scripting for routine automation.

*Formal appointment as System Administrator (Italian regulatory context).*

## Technologies & tools

- **Windows Server** and Windows client (10/11) — primary endpoint and
  server OS
- **Linux** (Debian/Ubuntu lineage) — server administration and Bash
  scripting
- **NinjaOne** — RMM platform for centralized fleet management
- **PowerShell**, **Python**, **Bash** — automation and custom scripting
- **OpenSSH**, **FTP**, **SFTP** — secure remote access and file transfer
- **TLS/HTTPS** certificate management
- **Microsoft Teams**, **Telegram** — alerting destinations
- **ITGlue** — RMM-integrated documentation
- Native Windows admin tooling: `systeminfo`, `msinfo32`, `wmic`,
  `sfc /scannow`, `chkdsk`, `driverquery`, `tasklist`, `taskkill`,
  `regedit`, `taskmgr`, `cleanmgr`, `diskpart`, `diskmgmt.msc`,
  `devmgmt.msc`, `compmgmt.msc`, `perfmon`, `eventvwr`, `services.msc`,
  `msconfig`, `netplwiz`
- Native network troubleshooting: `ipconfig /all`, `ping`, `tracert`,
  `netstat -ano`, `getmac`
- **Wine** — Windows application compatibility on Linux

## Responsibilities & operational scope

### General administration

- Monitoring of performance, KPIs, service levels, and IT systems /
  hardware obsolescence (e.g. company-wide PC replacement plan)
- Remote monitoring and proactive alerting systems
- Local and remote user support
- FTP, SSH, and SFTP server setup and maintenance
- Physical and virtual server maintenance and updates
- TLS/HTTPS certificate management and secure communication configuration
- Installation and management of clients, users, print queues, and
  peripherals
- Automation of repetitive tasks via custom scripting (Python, PowerShell)
- Windows-specific tuning: registry-level adjustments for preview, system
  hibernation, recycle-bin space limits, context-menu customization,
  preview handler management

### Linux/Unix administration

- Bash programming and scripting
- Linux directory structure and filesystem operations
- User and permission management
- Wine for Windows application compatibility on Linux hosts

### RMM operations (NinjaOne)

- Centralized management of all corporate endpoints and the Proxmox node
- Agent configuration and management on Windows, Linux, and macOS
- Proactive monitoring of logs, hardware and software performance, uptime,
  and service availability
- Custom alerting with delivery to Microsoft Teams and Telegram
- Advanced alerting for critical events (storage saturation, CPU/RAM
  pressure, system errors)
- Centralized patch management automation, maintenance scripts, and
  software deployment via custom policies
- Remote PowerShell and CMD scripting for non-disruptive operator
  interventions
- Encrypted endpoint and server backup procedures with validated restore
- RMM integration with internal technical documentation (ITGlue) for
  structured operational workflows
- Secure remote desktop operations with full activity traceability
- Failure prevention through proactive monitoring and corrective
  automation
- Analytics on corporate performance and IT resource usage
- RMM integration with ERP systems and business workflows

### Network and security responsibilities (operational overlap)

- Management of the complete corporate network, VPN, firewall, and
  network security
- Server and network-service installation, configuration, and updates
- Application of system security policies, firewall management, and
  service hardening
- Application lifecycle oversight, ensuring optimal operation at
  organizational scale
- Provisioning, maintenance, and update automation via scripts, patches,
  and policies
- Monitoring tool adoption and proposing optimizations to ensure
  consistent management policies
- Identification and testing of AI and automation solutions for
  efficiency, helpdesk, asset management, and knowledge sharing

## Projects & evidence

### NinjaOne RMM (Remote Machine Management)
<!-- graphify-evidence-id: bc8c22c83e21 -->

- **Source**: `ARCHITETTURA [HOSTNAME_56] 20052026_b5a58014.md`
- **Graph community**: 2

Remote Machine Management (RMM) centralizzata con Ninjaone In data 15/11/2024 [RIMOSSO] manda una mail per un’offerta da parte di Punto Informatica per riprendere un attimo in mano la situazione d

*Technology stack: to be enriched from source document.*

### File Extensions Visibility (NX).ps1
<!-- graphify-evidence-id: 67f5ca96e0b5 -->

- **Source**: `File Extensions Visibility (NX).ps1`
- **Graph community**: 38

﻿# ================================================================================ 📁 Hide File Extensions Plugin This plugin enables or disables the hiding of known file extensions in Explorer. #

*Technology stack: to be enriched from source document.*

### driverquery
<!-- graphify-evidence-id: a75cd6faac97 -->

- **Source**: `COMANDI UTILI PRONTI WINDOWS 11.txt`
- **Graph community**: 60

🔍 Info generali sul sistema Comando	Descrizione systeminfo	Mostra informazioni dettagliate su sistema operativo, RAM, BIOS, rete, aggiornamenti, ecc. msinfo32	Apre "Informazioni di sistema" con UI gra

*Technology stack: to be enriched from source document.*

### sfc /scannow
<!-- graphify-evidence-id: 41f41747e230 -->

- **Source**: `COMANDI UTILI PRONTI WINDOWS 11.txt`
- **Graph community**: 27

🔧 Diagnostica e strumenti utili Comando	Descrizione chkdsk	Controlla errori sul disco. sfc /scannow	Verifica l'integrità dei file di sistema. tasklist	Elenco dei processi attivi. taskkill /F /PID [num

*Technology stack: to be enriched from source document.*

### taskkill /F /PID
<!-- graphify-evidence-id: 47d6821a121d -->

- **Source**: `COMANDI UTILI PRONTI WINDOWS 11.txt`
- **Graph community**: 23

🔧 Diagnostica e strumenti utili Comando	Descrizione chkdsk	Controlla errori sul disco. sfc /scannow	Verifica l'integrità dei file di sistema. tasklist	Elenco dei processi attivi. taskkill /F /PID [num

*Technology stack: to be enriched from source document.*

### devmgmt.msc (Gestione dispositivi)
<!-- graphify-evidence-id: cdee01d4eb41 -->

- **Source**: `COMANDI UTILI PRONTI WINDOWS 11.txt`
- **Graph community**: 63

🔎 COMANDI DA “ESEGUI” (Windows + R) Comando	Descrizione msinfo32	Info di sistema dettagliate (hardware/software). dxdiag	Diagnostica DirectX e info su video, audio e input. devmgmt.msc	Gestione dispos

*Technology stack: to be enriched from source document.*

### Server Linux (Ubuntu)
<!-- graphify-evidence-id: 19062a04c29d -->

- **Source**: `DOCUWIKI.txt`
- **Graph community**: 10

Quindi praticamente DokuWiki funziona perfettamente su un server Linux perché è software open source scritto in PHP che utilizza file di testo semplice per memorizzare i dati e non richiede un databas

*Technology stack: to be enriched from source document.*

### Client SSH (OpenSSH Windows)
<!-- graphify-evidence-id: 286128d5b873 -->

- **Source**: `file BAT.txt`
- **Graph community**: 25

@echo off setlocal :: Chiede all'utente l'indirizzo SSH set /p ssh_target=Inserisci host SSH (es. [EMAIL_1]): :: Log file (nella cartella utente) set log_file=%USERPROFILE%\ssh_connection_log.

*Technology stack: to be enriched from source document.*

### Log Windows Event Viewer OpenSSH Operational
<!-- graphify-evidence-id: 2a9c1a6891b3 -->

- **Source**: `screenshot_03.png`
- **Graph community**: 3

*Evidence text to be enriched from source document.*

*Technology stack: to be enriched from source document.*

### Posta elettronica aziendale
<!-- graphify-evidence-id: 9bfddcf8a8fe -->

- **Source**: `Regolamento-utilizzo-strumenti-informatici.md`
- **Graph community**: 8

1. PRINCIPI GENERALI Il presente documento ha l’obiettivo di regolamentare l’accesso alla postazione di lavoro, l’utilizzo del telefono cellulare, di internet e della posta elettronica per gli utent

*Technology stack: to be enriched from source document.*

### Proxy server e file di log navigazione
<!-- graphify-evidence-id: 9c76847f4350 -->

- **Source**: `Regolamento-utilizzo-strumenti-informatici.md`
- **Graph community**: 8

- Al fine di prevenire il rischio di utilizzi impropri della rete, l’azienda adotta un sistema di filtri che riduce fortemente la possibilità di accesso a categorie di siti i cui contenuti sono stati

*Technology stack: to be enriched from source document.*

### ipconfig /all
<!-- graphify-evidence-id: f155be48b984 -->

- **Source**: `COMANDI UTILI PRONTI WINDOWS 11.txt`
- **Graph community**: 22

🌐 Rete Comando	Descrizione ipconfig /all	Dettagli completi sulle schede di rete. ping [indirizzo]	Verifica la connessione verso un host. tracert [indirizzo]	Mostra il percorso dei pacchetti di rete. n

*Technology stack: to be enriched from source document.*

### netstat -ano
<!-- graphify-evidence-id: 3c01419b7ec4 -->

- **Source**: `COMANDI UTILI PRONTI WINDOWS 11.txt`
- **Graph community**: 61

🌐 Rete Comando	Descrizione ipconfig /all	Dettagli completi sulle schede di rete. ping [indirizzo]	Verifica la connessione verso un host. tracert [indirizzo]	Mostra il percorso dei pacchetti di rete. n

*Technology stack: to be enriched from source document.*

### msconfig (Configurazione sistema)
<!-- graphify-evidence-id: 81b64f4c3338 -->

- **Source**: `COMANDI UTILI PRONTI WINDOWS 11.txt`
- **Graph community**: 64

🧰 Extra utili Gestione disco: diskmgmt.msc Connessioni di rete: ncpa.cpl Firewall: firewall.cpl Configurazione sistema (boot, avvio): msconfig Cartella avvio automatico: shell:startup Wise registry cl

*Technology stack: to be enriched from source document.*

### Rename Windows user (netplwiz + regedit)
<!-- graphify-evidence-id: b6c2ef3d6bd6 -->

- **Source**: `NOTES - Rinominare un utente in Windows in maniera completa.txt`
- **Graph community**: 5

Se si ha un PC formattato con Windows 11 dove ho un utente amministratore chiamato "Utente", rinominarlo cambia solo il nome visualizzato, non la cartella utente (C:\Users\Utente) che resterà così a m

*Technology stack: to be enriched from source document.*

### BIOS boot troubleshooting after USB removal
<!-- graphify-evidence-id: 4064c3aec1f2 -->

- **Source**: `14052025`

*Evidence text to be enriched from source document.*

*Technology stack: to be enriched from source document.*

### ipconfig /flushdns
<!-- graphify-evidence-id: 2855bf54889a -->

- **Source**: `flushare cache DNS da cmd.md`
- **Graph community**: 6

ipconfig /flushdns

*Technology stack: to be enriched from source document.*

### Ping su entrambi i nomi (test risoluzione)
<!-- graphify-evidence-id: 6d0891a2eabc -->

- **Source**: `ping entrambi i nomi.md`
- **Graph community**: 6

*Evidence text to be enriched from source document.*

*Technology stack: to be enriched from source document.*

### License Server (Studio network client licenses)
<!-- graphify-evidence-id: b49359ab4314 -->

- **Source**: `RWS Trados GroupShare 2020 SR1 CU7_Step 2_Technical Questionnaire_EN_Intrawelt.md`
- **Graph community**: 1

RWS Studio network client licenses need a Licensing Server component installed on a server. This can be the application server or a different one. Installation of the license server is not part of the

*Technology stack: to be enriched from source document.*

### Account RWS Intrawelt-Client (6058) e Intrawelt-Server (477664)
<!-- graphify-evidence-id: 2eb3133119d1 -->

- **Source**: `[HOSTNAME_8].md`
- **Graph community**: 8

Entrando dentro l’account RWS, si può notare la presenza di un account Intrawelt-Client (6058) e Intrawelt-Server (477664). Nello specifico, Intrawelt-Server (477664) ha la licenza Groupshare, che è l

*Technology stack: to be enriched from source document.*

### Script PowerShell aggiornamento server licenza su client (registro HKCU)
<!-- graphify-evidence-id: 2d7e70e8862b -->

- **Source**: `[HOSTNAME_8].md`
- **Graph community**: 7

Questo script non modifica il file hosts, ma aggiorna direttamente le impostazioni di licenza. Trados Studio e altre applicazioni SDL/RWS non leggono automaticamente le impostazioni di licenza da un f

*Technology stack: to be enriched from source document.*

### NinjaOne per distribuzione centralizzata impostazioni
<!-- graphify-evidence-id: 6e7606605a38 -->

- **Source**: `[HOSTNAME_8].md`
- **Graph community**: 7

Questo script non modifica il file hosts, ma aggiorna direttamente le impostazioni di licenza. Trados Studio e altre applicazioni SDL/RWS non leggono automaticamente le impostazioni di licenza da un f

*Technology stack: to be enriched from source document.*
