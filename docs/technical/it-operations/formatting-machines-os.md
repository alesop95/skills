# Formatting Machines & Operating Systems

## Overview

End-to-end workstation rebuild and OS recovery operations across diverse
hardware generations, from base hardware assembly through partition
schema design, driver management, and OS installation with custom
deployment media. Covers Windows and Linux distributions on both modern
and legacy machines.

## Technologies & tools

- **Medicat USB** — multi-tool recovery USB suite
- **Clonezilla** — disk imaging and cloning
- **gnome-disk-utility** — partition and volume operations
- **Ubuntu LTS**, **Xubuntu**, **anduinOS** — Linux distributions tested
  and deployed
- **Windows 11** — current target OS, including known-issue remediation
- Live OS environments for partitioning and recovery operations

## Responsibilities & operational scope

- Formatting of machines and installation of operating systems
- OS recovery from bootable devices with hardware/firmware compatibility
  validation
- Linux distribution testing and selection (anduinOS, Ubuntu LTS,
  Xubuntu)
- Experience with Medicat USB, Clonezilla, gnome-disk-utility, and live
  OS environments
- Windows 11 issue diagnosis and remediation
- Basic physical assembly of desktop workstation components (RAM, SSD,
  peripherals)
- Creation of customized installation media
- Advanced disk partition management on Linux and Windows
- Advanced driver management
- User account and system registry management
- Refurbishment of older machines: partition schema design, hardware-
  software compatibility analysis, legacy driver sourcing
- Windows Update, hotfix, and hardware obsolescence management

## Projects & evidence

### GNOME Disk Utility
<!-- graphify-evidence-id: a765befa0f61 -->

- **Source**: `Lanciare gnome-disk-utility da una live (alternativa cloneZilla)_d936952b.md`
- **Graph community**: 3

Lanciare gnome-disk-utility da una live di Ubuntu Per avviare la sessione live di Ubuntu da una chiavetta USB e usare GNOME Disks Utility per creare un'immagine del disco si possono seguire questi pas

*Technology stack: to be enriched from source document.*

### Clonezilla
<!-- graphify-evidence-id: a138a15e1633 -->

- **Source**: `Lanciare gnome-disk-utility da una live (alternativa cloneZilla)_d936952b.md`
- **Graph community**: 3

Lanciare gnome-disk-utility da una live di Ubuntu Per avviare la sessione live di Ubuntu da una chiavetta USB e usare GNOME Disks Utility per creare un'immagine del disco si possono seguire questi pas

*Technology stack: to be enriched from source document.*

### Startup Disk Creator
<!-- graphify-evidence-id: 8e1fcc54dbe9 -->

- **Source**: `Lanciare gnome-disk-utility da una live (alternativa cloneZilla)_d936952b.md`
- **Graph community**: 3

Lanciare gnome-disk-utility da una live di Ubuntu Per avviare la sessione live di Ubuntu da una chiavetta USB e usare GNOME Disks Utility per creare un'immagine del disco si possono seguire questi pas

*Technology stack: to be enriched from source document.*

### dd (Disk Dump)
<!-- graphify-evidence-id: e9a085b013e0 -->

- **Source**: `comando_ubuntu_locale.txt`
- **Graph community**: 3

sudo dd if=/dev/sdX of=/percorso/ubuntu_backup.img bs=4M status=progress "/dev/sdX" = il percorso del disco da copiare come .img "/percorso"	= il percorso di destinazione del clone

*Technology stack: to be enriched from source document.*

### Ubuntu Live USB
<!-- graphify-evidence-id: 45544fc21220 -->

- **Source**: `Lanciare gnome-disk-utility da una live (alternativa cloneZilla)_d936952b.md`
- **Graph community**: 3

Lanciare gnome-disk-utility da una live di Ubuntu Per avviare la sessione live di Ubuntu da una chiavetta USB e usare GNOME Disks Utility per creare un'immagine del disco si possono seguire questi pas

*Technology stack: to be enriched from source document.*

### Ubuntu 24.04 LTS Noble Numbat
<!-- graphify-evidence-id: 75c52345e2e3 -->

- **Source**: `Note.txt`
- **Graph community**: 6

🔸 Ubuntu 25.04 "Plucky Puffin" (versione intermedia) Rilasciata il: 17 aprile 2025 Supporto: 9 mesi, fino a gennaio 2026 Novità principali: Kernel Linux 6.8, GNOME 48, supporto predefinito per JPEG XL

*Technology stack: to be enriched from source document.*

### Ubuntu 25.04 Plucky Puffin
<!-- graphify-evidence-id: c1f04a579602 -->

- **Source**: `Note.txt`
- **Graph community**: 6

🔸 Ubuntu 25.04 "Plucky Puffin" (versione intermedia) Rilasciata il: 17 aprile 2025 Supporto: 9 mesi, fino a gennaio 2026 Novità principali: Kernel Linux 6.8, GNOME 48, supporto predefinito per JPEG XL

*Technology stack: to be enriched from source document.*

### AnduinOS NVMe LBA 512-byte requirement
<!-- graphify-evidence-id: 20ece63f8e0e -->

- **Source**: `doc.txt`
- **Graph community**: 6

https://[RIMOSSO]/ | |	Installing AnduinOS | |	|	https://[RIMOSSO]/Install/System-Requirements.html |	|	System requirements for the best experience: |	|	Component Requirement |	|	Ar

*Technology stack: to be enriched from source document.*

### Rufus dd mode (for AnduinOS USB)
<!-- graphify-evidence-id: c170bd25736c -->

- **Source**: `doc.txt`
- **Graph community**: 6

https://[RIMOSSO]/ | |	Installing AnduinOS | |	|	https://[RIMOSSO]/Install/System-Requirements.html |	|	System requirements for the best experience: |	|	Component Requirement |	|	Ar

*Technology stack: to be enriched from source document.*

### Secure Boot (UEFI)
<!-- graphify-evidence-id: 979d7e7b7f28 -->

- **Source**: `doc.txt`
- **Graph community**: 6

https://[RIMOSSO]/ | |	Installing AnduinOS | |	|	https://[RIMOSSO]/Install/System-Requirements.html |	|	System requirements for the best experience: |	|	Component Requirement |	|	Ar

*Technology stack: to be enriched from source document.*

### Windows 11 ISO download
<!-- graphify-evidence-id: a32023f41a9a -->

- **Source**: `Clever Windows 11 formatting_c52d66b5.md`
- **Graph community**: 0

The .iso file download and Product key Iso file download To download the operating system, starting from the official https://www.microsoft.com/it-it/software-download/windows11 link and go to

*Technology stack: to be enriched from source document.*

### Windows 11 Home
<!-- graphify-evidence-id: 63e73d3d0b4e -->

- **Source**: `DIFFERENZE TRA WINDOWS 11 HOME, EDUCATION, PRO (e la loro versione N).txt`
- **Graph community**: 0

Windows 11 è disponibile in diverse edizioni, ognuna con caratteristiche specifiche. Ecco un confronto tra Windows 11 Home, Pro e Education: ___________________________________________________________

*Technology stack: to be enriched from source document.*

### Windows 11 Pro
<!-- graphify-evidence-id: 7c09078d3ebb -->

- **Source**: `DIFFERENZE TRA WINDOWS 11 HOME, EDUCATION, PRO (e la loro versione N).txt`
- **Graph community**: 0

Windows 11 è disponibile in diverse edizioni, ognuna con caratteristiche specifiche. Ecco un confronto tra Windows 11 Home, Pro e Education: ___________________________________________________________

*Technology stack: to be enriched from source document.*

### Windows 11 Education
<!-- graphify-evidence-id: 33690f1063da -->

- **Source**: `DIFFERENZE TRA WINDOWS 11 HOME, EDUCATION, PRO (e la loro versione N).txt`
- **Graph community**: 0

Windows 11 è disponibile in diverse edizioni, ognuna con caratteristiche specifiche. Ecco un confronto tra Windows 11 Home, Pro e Education: ___________________________________________________________

*Technology stack: to be enriched from source document.*

### Windows 11 N editions (no Media Pack)
<!-- graphify-evidence-id: 67020c882410 -->

- **Source**: `DIFFERENZE TRA WINDOWS 11 HOME, EDUCATION, PRO (e la loro versione N).txt`
- **Graph community**: 0

Se si ha bisogno di queste funzionalità, si può installare il Media Feature Pack disponibile gratuitamente da Microsoft. Quindi, le versioni "N" sono come un "template" vergine senza le funzionalità m

*Technology stack: to be enriched from source document.*

### Media Feature Pack
<!-- graphify-evidence-id: f16cb1717b23 -->

- **Source**: `DIFFERENZE TRA WINDOWS 11 HOME, EDUCATION, PRO (e la loro versione N).txt`
- **Graph community**: 0

Se si ha bisogno di queste funzionalità, si può installare il Media Feature Pack disponibile gratuitamente da Microsoft. Quindi, le versioni "N" sono come un "template" vergine senza le funzionalità m

*Technology stack: to be enriched from source document.*

### diskmgmt.msc (Disk Management)
<!-- graphify-evidence-id: b10a93df037b -->

- **Source**: `NOTES - La gestione delle partizioni del disco.txt`
- **Graph community**: 4

diskmgmt.msc Per aprire l'utility di Gestione Disco e individuare ad esempio la partizione che contiene il vecchio sistema operativo Windows. Nel momento in cui si eliminasse una partizione con "Elimi

*Technology stack: to be enriched from source document.*

### diskpart utility
<!-- graphify-evidence-id: d1e697941c00 -->

- **Source**: `NOTES - La gestione delle partizioni del disco.txt`
- **Graph community**: 4

Per aprire l'utility di Gestione Disco e individuare ad esempio la partizione che contiene il vecchio sistema operativo Windows. Nel momento in cui si eliminasse una partizione con "Elimina volume" qu

*Technology stack: to be enriched from source document.*

### MBR 4-partition limit
<!-- graphify-evidence-id: 995ae049ad95 -->

- **Source**: `Penso dipenda dal fatto che un disco MBR non può avere più di 4 partizioni.txt`
- **Graph community**: 4

*Evidence text to be enriched from source document.*

*Technology stack: to be enriched from source document.*

### Product key / slmgr /xpr
<!-- graphify-evidence-id: b509fc232309 -->

- **Source**: `Clever Windows 11 formatting_c52d66b5.md`
- **Graph community**: 0

and the product key https://support.microsoft.com/en-us/windows/find-your-windows-product-key-aaa2bf69-7b2b-9f13-f581-a806abf0a886 (a 25-character key that unlocks and activates the correct edition of

*Technology stack: to be enriched from source document.*

### Windows Hardware Fingerprinting (HWID)
<!-- graphify-evidence-id: 355ed371faa6 -->

- **Source**: `Clever Windows 11 formatting_c52d66b5.md`
- **Graph community**: 0

When you install Windows 11, the system checks your PC's hardware, and if it finds a match with your stored product key, it will automatically activate Windows without requiring you to manually enter

*Technology stack: to be enriched from source document.*

### dism /Get-WimInfo ISO inspection
<!-- graphify-evidence-id: ae8de487e3a2 -->

- **Source**: `Clever Windows 11 formatting_c52d66b5.md`
- **Graph community**: 0

Basically, Windows generates a hardware ID (HWID) as a unique fingerprint based on several hardware components, such as Motherboard (biggest factor), CPU, TPM, Disk serial number and sometimes MAC add

*Technology stack: to be enriched from source document.*

### Rufus 4.7 writing MBR for Ubuntu 24.04.2 LTS amd64 ISO (MBR partition scheme, BIOS or UEFI)
<!-- graphify-evidence-id: 337f8bbcf0f0 -->

- **Source**: `rufus_settings_example.jpg`
- **Graph community**: 6

*Evidence text to be enriched from source document.*

*Technology stack: to be enriched from source document.*

### Windows 11 installer: Seleziona il percorso di installazione - partition list (Disk 0 P1-5 + USB)
<!-- graphify-evidence-id: 0d8bed8bf272 -->

- **Source**: `2. formatta partizione.jpg`
- **Graph community**: 0

*Evidence text to be enriched from source document.*

*Technology stack: to be enriched from source document.*

### Windows 11 Pronto per l'installazione: Installa Windows 11 Pro + Non conservare nulla
<!-- graphify-evidence-id: f3ba7db17a2e -->

- **Source**: `3. Installa Windows 11 (Pro) + Non conservare nulla (controlla le specifiche del dispositivo).jpg`
- **Graph community**: 0

*Evidence text to be enriched from source document.*

*Technology stack: to be enriched from source document.*

### Win11 installer partition picker: multi-disk layout with 'Errore selezione partizione' popup
<!-- graphify-evidence-id: 34bd47b80c16 -->

- **Source**: `1.jpg`
- **Graph community**: 4

*Evidence text to be enriched from source document.*

*Technology stack: to be enriched from source document.*

### Win11 installation in progress at 5%, multiple reboots warning on LG Flatron monitor
<!-- graphify-evidence-id: 86653f6f9567 -->

- **Source**: `5.jpg`
- **Graph community**: 4

*Evidence text to be enriched from source document.*

*Technology stack: to be enriched from source document.*

### Linux live USB disk-clone workflow
<!-- graphify-evidence-id: 57ed8d1c0308 -->

- **Source**: `Lanciare gnome-disk-utility da una live (alternativa cloneZilla)_d936952b.md`

*Evidence text to be enriched from source document.*

*Technology stack: to be enriched from source document.*

### Rufus Xubuntu USB creation full workflow
<!-- graphify-evidence-id: 9cf86279f960 -->

- **Source**: `13052025`

*Evidence text to be enriched from source document.*

*Technology stack: to be enriched from source document.*

### Recycle bin cap (basic)
<!-- graphify-evidence-id: 7c5dab98e971 -->

- **Source**: `recycle_bin_cap.ps1`
- **Graph community**: 28

Ottieni il percorso del registro di sistema per il cestino $recycleBinRegPath = "HKCU:\Software\Microsoft\Windows\CurrentVersion\Explorer\BitBucket\Volume" Ottieni tutte le sottochiavi del registr

*Technology stack: to be enriched from source document.*

### Recycle bin cap (with volume names)
<!-- graphify-evidence-id: 5de68ab5ef2b -->

- **Source**: `recycle_bin_cap_printNames.ps1`
- **Graph community**: 28

Ottieni il percorso del registro di sistema per il cestino $recycleBinRegPath = "HKCU:\Software\Microsoft\Windows\CurrentVersion\Explorer\BitBucket\Volume" Ottieni tutte le sottochiavi del registr

*Technology stack: to be enriched from source document.*

### Wechoid Locking Utility (codici blocco hardware)
<!-- graphify-evidence-id: b72a16f89c8f -->

- **Source**: `[HOSTNAME_8].md`
- **Graph community**: 8

Locking Utility (Wechoid): Genera codici di blocco per attivare le licenze di rete. Wechoid mostra le informazioni di blocco hardware, come l'indirizzo MAC, l'ID del disco rigido, e altre caratteristi

*Technology stack: to be enriched from source document.*
