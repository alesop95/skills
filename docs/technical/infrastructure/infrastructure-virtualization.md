# Infrastructure & Virtualization

## Overview

Design, deployment, and operations of on-premise virtualization platforms,
from bare-metal cluster bootstrap to day-2 lifecycle management of guest
workloads. Covers hypervisor selection and configuration, virtual networking
and shared storage, high availability, and automation of routine
maintenance.

## Technologies & tools

- **Proxmox VE** (8.3.4) on Debian-based hosts — primary on-premise hypervisor
- **VMware vSphere** — alternative enterprise hypervisor
- **Postfix** + **mailutils** — automated email alerting from hypervisor hosts
- **cron** — scheduled health checks and resource notifications
- **Bash** scripting for VM lifecycle automation
- Windows Server and Linux as guest operating systems

## Responsibilities & operational scope

- Full hypervisor deployment from scratch, including virtualized network
  resource management, logical pool organization, NAT configuration, and
  shared storage integration
- Cluster setup with high availability (HA) and shared storage
- Setup and ongoing management of Windows Server and Linux guest VMs
- Linux VM migration and long-term maintainability
- Development of automation scripts for VM lifecycle operations: provisioning,
  backups, snapshots, and routine maintenance tasks
- Monitoring of VM-specific resources via Postfix/mailutils email alerts and
  scheduled cron-based health checks on critical VMs

## Projects & evidence

### Windows 11 bloatware removal
<!-- graphify-evidence-id: f1ebd87db593 -->

- **Source**: `Clever Windows 11 formatting_c52d66b5.md`
- **Graph community**: 11

(TBC) Restarting the laptop booting the volume with .iso aaaaaaaaaaa talk about the actual installation of the operating system after the first boot here aaaaaaaaaaa After the installation Wi

*Technology stack: to be enriched from source document.*

### HP ProLiant ML370 G5 (dismesso)
<!-- graphify-evidence-id: f1573e8d6139 -->

- **Source**: `ARCHITETTURA [HOSTNAME_56] 20052026_b5a58014.md`
- **Graph community**: 7

Lanciando la macchina, quindi, funziona e si può anche fare l’accesso. Si può seguire la stessa procedura per le altre macchine Linux – vedere anche sezione Migrazione VM progetti pending [RIMOSSO] su

*Technology stack: to be enriched from source document.*

### VM W2012_licserver (Windows Server 2012, dismessa)
<!-- graphify-evidence-id: cd6fd54d8e73 -->

- **Source**: `ARCHITETTURA [HOSTNAME_56] 20052026_b5a58014.md`
- **Graph community**: 7

- Multitserver(nome VM: Win 2008 Srv ) - Accesso via “Desktop remoto” - IP:[IP_85] - License Server SDL 2007/2009/20011 - ABBYY License server - DOMV new: - Ospita gli altri domini web e i blog

*Technology stack: to be enriched from source document.*

### VM W2012_bioserver (Windows Server 2012)
<!-- graphify-evidence-id: 8255141a3321 -->

- **Source**: `ARCHITETTURA [HOSTNAME_56] 20052026_b5a58014.md`
- **Graph community**: 7

- Multitserver(nome VM: Win 2008 Srv ) - Accesso via “Desktop remoto” - IP:[IP_85] - License Server SDL 2007/2009/20011 - ABBYY License server - DOMV new: - Ospita gli altri domini web e i blog

*Technology stack: to be enriched from source document.*

### [HOSTNAME_5] [HOSTNAME_71] (Windows Server 2022, nuova)
<!-- graphify-evidence-id: 06733286b61e -->

- **Source**: `ARCHITETTURA [HOSTNAME_56] 20052026_b5a58014.md`
- **Graph community**: 7

Nel nostro caso è troppo vecchia. Si può provare ad importare una VM dentro passando sempre per lo storage condiviso del NAS come visto nella sezione precedente. Inoltre, per la migrazione delle macch

*Technology stack: to be enriched from source document.*

### BioStar 2 (sistema controllo accessi Suprema)
<!-- graphify-evidence-id: e4194e5b3612 -->

- **Source**: `ARCHITETTURA [HOSTNAME_56] 20052026_b5a58014.md`
- **Graph community**: 7

- È una funzionalità che consente di rendere un dispositivo fisico dell'host (come una scheda USB, una GPU, un dispositivo PCIe, o una periferica hardware) accessibile direttamente all'interno di un c

*Technology stack: to be enriched from source document.*

### Suprema BioEntry W2 (lettore biometrico)
<!-- graphify-evidence-id: ce58c54de3ad -->

- **Source**: `ARCHITETTURA [HOSTNAME_56] 20052026_b5a58014.md`
- **Graph community**: 7

Il dispositivo è BioEntry W2 | Biostar 2 della Suprema, modello [HOSTNAME_78] con FCC ID: [HOSTNAME_79]. Il reset delle impostazioni di rete lo fa, il reset delle impostazioni di fabbrica non lo fa. Nonostan

*Technology stack: to be enriched from source document.*

### SecureIO2 (relais serratura RS485)
<!-- graphify-evidence-id: 325ad41ab9d2 -->

- **Source**: `ARCHITETTURA [HOSTNAME_56] 20052026_b5a58014.md`
- **Graph community**: 7

Il SecureIO2 7887066119 remotizza e virtualizza la serratura così anche dall'esterno tramite il protocollo seriale RS485 si apre la serratura e funziona. Infatti, il lettore ingresso e uscita sono due

*Technology stack: to be enriched from source document.*

### Windows ACL + Autorizzazioni cartella avanzate (QTS)
<!-- graphify-evidence-id: 553ea2091afb -->

- **Source**: `ARCHITETTURA [HOSTNAME_56] 20052026_b5a58014.md`
- **Graph community**: 10

Di default e gestire il tutto con l’assegnazione a gruppi specifici che modificano il privilegio di un utente a seconda della sua assegnazione. Sono stati creati tutti gli utenti che alla data 20/06/2

*Technology stack: to be enriched from source document.*

### Proxmox Backup Server (opzione riuso HPX1400)
<!-- graphify-evidence-id: 6a8b57037437 -->

- **Source**: `ARCHITETTURA [HOSTNAME_56] 20052026_b5a58014.md`
- **Graph community**: 10

Buttare completamente via il NAS (aborted) Si ha il PRO del risparmio di energia elettrica (anche se consuma meno degli altri, in un anno pesa). Valutando ciò, Il NAS HP StorageWorks X1400 G2 è dotato

*Technology stack: to be enriched from source document.*

### Windows Desktop Remoto (RDP TCP 3389)
<!-- graphify-evidence-id: ba32c324f9c7 -->

- **Source**: `shared`
- **Graph community**: 4

*Evidence text to be enriched from source document.*

*Technology stack: to be enriched from source document.*

### Procedura abilitare RDP in Windows 11 (PC controllato)
<!-- graphify-evidence-id: fdd6c0bf871a -->

- **Source**: `abilitare RDP in Windows 11 sul PC che deve essere controllato_e3346c46.md`
- **Graph community**: 4

*Evidence text to be enriched from source document.*

*Technology stack: to be enriched from source document.*

### Requisito: Windows 11 Pro / Enterprise / Education (Home non supporta host RDP)
<!-- graphify-evidence-id: b6bf15ab0daf -->

- **Source**: `abilitare RDP in Windows 11 sul PC che deve essere controllato_e3346c46.md`
- **Graph community**: 4

*Evidence text to be enriched from source document.*

*Technology stack: to be enriched from source document.*

### Windows Update Tamer.ps1
<!-- graphify-evidence-id: 5b54ba7266de -->

- **Source**: `Windows Update Tamer.ps1`
- **Graph community**: 24

"Show Info" { Write-Output "[INFO] Windows Update Tamer" Write-Output "---------------------------------------------------" Write-Output "Control Windows Update without opening

*Technology stack: to be enriched from source document.*

### Ensure-UxKey()
<!-- graphify-evidence-id: 669215a1c219 -->

- **Source**: `Windows Update Tamer.ps1`
- **Graph community**: 24

function Ensure-UxKey { $ux = "HKLM:\SOFTWARE\Microsoft\WindowsUpdate\UX\Settings" if (-not (Test-Path $ux)) { New-Item -Path $ux -Force | Out-Null } return $ux } function Unlock-PauseUx {

*Technology stack: to be enriched from source document.*

### Unlock-PauseUx()
<!-- graphify-evidence-id: f2f69e2d53f8 -->

- **Source**: `Windows Update Tamer.ps1`
- **Graph community**: 24

function Unlock-PauseUx { $pol = "HKLM:\SOFTWARE\Policies\Microsoft\Windows\WindowsUpdate" if (Test-Path $pol) { Remove-ItemProperty -Path $pol -Name "SetDisablePauseUXAccess" -ErrorAc

*Technology stack: to be enriched from source document.*

### MoinMoin Wiki
<!-- graphify-evidence-id: 168e6d5f4a7d -->

- **Source**: `DOCUWIKI.txt`
- **Graph community**: 10

https://www.dokuwiki.org/dokuwiki https://www.dokuwiki.org/it:features Quindi praticamente DokuWiki funziona perfettamente su un server Linux perché è software open source scritto in PHP che utilizza

*Technology stack: to be enriched from source document.*

### PHP + Apache/Nginx
<!-- graphify-evidence-id: d331bb543a88 -->

- **Source**: `DOCUWIKI.txt`
- **Graph community**: 10

Quindi praticamente DokuWiki funziona perfettamente su un server Linux perché è software open source scritto in PHP che utilizza file di testo semplice per memorizzare i dati e non richiede un databas

*Technology stack: to be enriched from source document.*

### Storage su file di testo (no DB)
<!-- graphify-evidence-id: c7134ee6cd14 -->

- **Source**: `DOCUWIKI.txt`
- **Graph community**: 10

Quindi praticamente DokuWiki funziona perfettamente su un server Linux perché è software open source scritto in PHP che utilizza file di testo semplice per memorizzare i dati e non richiede un databas

*Technology stack: to be enriched from source document.*

### Personalizzazione menu contestuale Windows 11
<!-- graphify-evidence-id: 98328a78191a -->

- **Source**: `EasycontextMenu.txt`

*Evidence text to be enriched from source document.*

*Technology stack: to be enriched from source document.*

### Procedura ricostruzione storico SSH su Windows 10+
<!-- graphify-evidence-id: d8cb95719ed5 -->

- **Source**: `Ricostruire storico SSH in Windows (da 10 in poi)`

*Evidence text to be enriched from source document.*

*Technology stack: to be enriched from source document.*

### VPN aziendale Intrawelt (server [IP_2])
<!-- graphify-evidence-id: b05e9c5810e1 -->

- **Source**: `shared`
- **Graph community**: 4

*Evidence text to be enriched from source document.*

*Technology stack: to be enriched from source document.*

