# Advanced Helpdesk

## Overview

First and second-level technical support for local and remote users, covering diagnosis of software and configuration issues, device provisioning, license operations, and infrastructure-side troubleshooting. Includes hardware lifecycle planning and standardized OS deployment workflows across heterogeneous workstation profiles.

## Technologies & tools

- **nLite** — custom Windows bootable media builds
- Linux live environments for GPT partitioning and pre-install operations
- **ABBYY License Manager**, **Trados**, **Biostar**, **TimeWalker** — managed business applications
- UPS systems for electrical continuity
- Antivirus / endpoint protection (see also Cybersecurity & IT Governance)

## Responsibilities & operational scope

- First-level technical support for local and remote users
- Diagnosis of issues across software, LAN, WAN configuration, and user access
- End-user device, user access, and system troubleshooting
- Client configuration and setup
- Automation and improvement of onboarding/offboarding processes for scalability and user satisfaction
- Collaboration with internal teams (project management) to ensure continuity, reliability, and performance of infrastructure services
- Standardized device provisioning and OS deployment workflows using custom bootable media: nLite-based Windows builds, Linux live environments for GPT partitioning, multi-hardware imaging validation, ensuring full hardware compatibility and reducing setup time and configuration errors across workstation profiles
- Hardware lifecycle management: company-wide PC replacement plan to phase out obsolete Intel pre-7th gen systems and ensure full Windows 11 compliance, improving reliability and long-term support
- Server and service performance monitoring
- System log management and event analysis
- Software license management and migration (ABBYY, Trados, Biostar, TimeWalker)
- UPS and electrical continuity management
- ISP provider migration and internal settings management

## Projects & evidence

### Win11 install media creation flow
<!-- graphify-evidence-id: bc704f7d52d9 -->

- **Source**: `Clever Windows 11 formatting_c52d66b5.md`

*Evidence text to be enriched from source document.*

*Technology stack: to be enriched from source document.*

### Windows 11 install + OOBE + first updates flow
<!-- graphify-evidence-id: aea02a277b06 -->

- **Source**: `Windows 11`

*Evidence text to be enriched from source document.*

*Technology stack: to be enriched from source document.*

### Timewalker (software timbrature)
<!-- graphify-evidence-id: 1c226707400b -->

- **Source**: `ARCHITETTURA [HOSTNAME_56] 20052026_b5a58014.md`
- **Graph community**: 7

Le timbrature staranno su un database SQL da poter esportare su un’altra macchina o su un database interno. Vedere chiamando loro se BioStar ha una procedura di esportazione > importazione. - Installa

*Technology stack: to be enriched from source document.*

### Trados License Manager (RWS)
<!-- graphify-evidence-id: 733246ff5fa3 -->

- **Source**: `ARCHITETTURA [HOSTNAME_56] 20052026_b5a58014.md`
- **Graph community**: 7

Nel nostro caso è troppo vecchia. Si può provare ad importare una VM dentro passando sempre per lo storage condiviso del NAS come visto nella sezione precedente. Inoltre, per la migrazione delle macch

*Technology stack: to be enriched from source document.*

### ABBYY FineReader 15 License Server
<!-- graphify-evidence-id: ff60c1c8c941 -->

- **Source**: `ARCHITETTURA [HOSTNAME_56] 20052026_b5a58014.md`
- **Graph community**: 7

E dentro è stata messa la cartella “ABBYY FineReader 15 License Server”: Che è stata presa da C:\Program Files (x86) dell’utente locale di [PERSONA_7]. La descrizione della procedura di Migrazione

*Technology stack: to be enriched from source document.*

### Gruppo utenti utili-users
<!-- graphify-evidence-id: 0b7339be8a10 -->

- **Source**: `ARCHITETTURA [HOSTNAME_56] 20052026_b5a58014.md`
- **Graph community**: 10

Considerazioni su migrazione Quello che serve sapere prima di procedere con una migrazione è che il [HOSTNAME_72] monta un sistema RAID gestito da QTS su architettura x86, mentre il TS-435XeU-4G usa un'arch

*Technology stack: to be enriched from source document.*

### Post-install essentials.ps1
<!-- graphify-evidence-id: 992b683f7231 -->

- **Source**: `Post-install essentials.ps1`
- **Graph community**: 29

﻿# Post-install Essentials – quick launcher for Windows tools (+ .NET 3.5) Host: embedded Category: Post Options: Open Windows Features (classic); Open Optional features (Settings); Install .NET

*Technology stack: to be enriched from source document.*

### Vianova [HOSTNAME_70] (gruppo di continuita)
<!-- graphify-evidence-id: 4827dd3d9f8f -->

- **Source**: `ARCHITETTURA [HOSTNAME_56] 20052026_b5a58014.md`
- **Graph community**: 2

Per qualsiasi necessità può contattare il nostro Servizio Clienti al numero gratuito 145 tutti i giorni dalle 8:00 alle 22:00, comprese le festività. A seguito della migrazione completa da connettivit

*Technology stack: to be enriched from source document.*

### Pacchetto di progetto Trados Studio
<!-- graphify-evidence-id: 404296bc59e8 -->

- **Source**: `2022-12-05_Procedura_Creazione_di_un_progetto_su_Studio.md`
- **Graph community**: 0

CREAZIONE DI UN PROGETTO CON TRADOS STUDIO Come si crea la cartella di un progetto?	3 Come si salva il materiale inviato dal cliente?	4

*Technology stack: to be enriched from source document.*

### Secondo giro installazioni Trados 2024 e pulizia postazioni
<!-- graphify-evidence-id: ec38ba0b3f3f -->

- **Source**: `secondo_giro installazioni Trados 2024 (e disinstallazione_pulizia postazioni).md`
- **Graph community**: 4

Aggiornamento Trados 2024: [PERSONA_5] [PERSONA_15] [RIMOSSO] + componente per Trados che serve per il World Server di [RIMOSSO] [RIMOSSO] [RIMOSSO] (pending) [RIMOSSO] [RIMOSSO] [RIMOSSO] [RIMOSSO] [RIMOSSO] B.

*Technology stack: to be enriched from source document.*

### RWS Trados GroupShare 2020 SR1 CU7 Technical Questionnaire
<!-- graphify-evidence-id: f6eb0d62008a -->

- **Source**: `RWS Trados GroupShare 2020 SR1 CU7_Step 2_Technical Questionnaire_EN_Intrawelt.md`
- **Graph community**: 1

RWS Trados GroupShare 2020 SR1 Technical Questionnaire Professional Services

*Technology stack: to be enriched from source document.*

### SDL License Server Manager (v18.0.79)
<!-- graphify-evidence-id: 717b3dcdd684 -->

- **Source**: `[HOSTNAME_8].md`
- **Graph community**: 1

Per ulteriori problematiche vedere il file SDL_License_Server_Manager_User_Guide.pdf . Il PC di [RIMOSSO] ha l’accesso già salvato in rdp. Installazione SDL License server manager su nuovo server e

*Technology stack: to be enriched from source document.*

### Trados License Manager (online activation)
<!-- graphify-evidence-id: eb851624c964 -->

- **Source**: `[HOSTNAME_8].md`
- **Graph community**: 1

Delle tre utility è proprio il Trados License Manager da utilizzare, in generale per fare una (de-)activation online https://gateway.rws.com/csm?sys_kb_id=9acd66e01b0f9a50772c0dcad34bcb07&id=kb_articl

*Technology stack: to be enriched from source document.*

### Trial license Trados Studio 2024 (30gg)
<!-- graphify-evidence-id: 0178d8dc19d3 -->

- **Source**: `[HOSTNAME_8].md`
- **Graph community**: 4

Nel frattempo, si era scritto alla [RIMOSSO] e ci facciamo mandare altre licenze aggiuntive di prova per stare coperti (se possibile di una settimana) appena si hanno le suddette. Una volta settate le

*Technology stack: to be enriched from source document.*

### Deployment Trados 2024 sui PM Intrawelt (uninstall 2022 + install 2024 + trial)
<!-- graphify-evidence-id: 65d6d88fb86d -->

- **Source**: `secondo_giro installazioni Trados 2024 (e disinstallazione_pulizia postazioni).md`

*Evidence text to be enriched from source document.*

*Technology stack: to be enriched from source document.*
