# Microsoft 365 Business

## Overview

Tenant-level administration and advanced usage of the Microsoft 365
Business suite across all major services, with attention to security
posture, automation, and integration with external systems. Covers
Exchange, SharePoint, Teams, OneDrive, Power Automate, and Purview as
operational tools rather than as end-user applications.

## Technologies & tools

- **Microsoft 365 Business** — full tenant administration
- **Exchange Online** — mail flow, eDiscovery, policy management
- **SharePoint Online**, **Teams**, **OneDrive** — collaboration stack
- **Power Automate** — workflow automation with API triggers
- **Microsoft Purview** — audit log management and data analysis
- **Azure AD / Microsoft Entra** — Client ID, Client Secret, Tenant ID
  for app registrations
- **Power Query** — eDiscovery dataset export and analysis
- VBA, Office macros, Python-inside-Excel, Google Apps Script

## Responsibilities & operational scope

- Microsoft 365 Business expertise across the full suite
- Security policy and best-practice enforcement (e.g. MFA Enforcement)
- Advanced usage of the Office suite, macros, VBA, and scripting
- Management of advanced plugins and developer options (e.g. Python
  inside Excel)
- Structured, modular, hyperlinked content organization with custom
  styles, accessibility protection, document control, and anonymization

### Exchange

- Setting private mail servers and custom notification alerts across
  services
- Mailbox delegation and forwarding configuration
- Mailbox archival, tracing, and deletion
- Policy customization
- Phishing-threat email data analysis
- Reverse-DNS issue resolution for client domains
- Inbound/outbound external domain management
- eDiscovery operations

### SharePoint, Teams, and OneDrive

- SharePoint, Teams, and OneDrive sharing and integration
- Running multiple OneDrive instances on a single workstation
- Integration with external services via API
- Storage and folder organization across multiple teams

### Teams (admin)

- Teams Admin Center operations
- Shift and permission management, team creation

### Power Automate

- Pipeline design and scripting automation (Python integration)
- Advanced triggering patterns
- Client ID / Client Secret / Tenant ID for Azure AD / Microsoft Entra
  connectivity
- Custom flows for corporate attendance management
- eDiscovery dataset export and data analysis via Power Query

### Purview

- Custom audit log management
- Data processing via Power Query

## Projects & evidence

### Microsoft Entra ID
<!-- graphify-evidence-id: 7dc9d0eb1312 -->

- **Source**: `ARCHITETTURA [HOSTNAME_56] 20052026_b5a58014.md`
- **Graph community**: 12

L’mportante è che non ci siano dentro configurazioni di altri firewall perché sennò se la carico sputtana. La serie Flex non poteva essere caricata su Nebula per una questione di firmware (non abilita

*Technology stack: to be enriched from source document.*

### Microsoft 365 / Exchange Online
<!-- graphify-evidence-id: f570e752c014 -->

- **Source**: `ARCHITETTURA [HOSTNAME_56] 20052026_b5a58014.md`
- **Graph community**: 12

[RIMOSSO] non c’è più, Posta non c’è più (si utilizza Exchange online). Viene utilizzato soltanto uno dei tre: Con Mantis che rispondeVA al [IP_22] sul G6 e ora risponde allo stesso indirizzo IP

*Technology stack: to be enriched from source document.*

### Microsoft Authenticator
<!-- graphify-evidence-id: 11c47c6e08cc -->

- **Source**: `Authenticator e Entra ID.txt`
- **Graph community**: 4

L’immagine mostra una schermata in cui viene richiesto il codice generato da Microsoft Authenticator, ma sul dispositivo nuovo non appare alcun account configurato. Questo scenario, unito all’errore 5

*Technology stack: to be enriched from source document.*

### Microsoft Entra ID (Azure AD)
<!-- graphify-evidence-id: dc5ed7f58b40 -->

- **Source**: `Authenticator e Entra ID.txt`
- **Graph community**: 4

L’immagine mostra una schermata in cui viene richiesto il codice generato da Microsoft Authenticator, ma sul dispositivo nuovo non appare alcun account configurato. Questo scenario, unito all’errore 5

*Technology stack: to be enriched from source document.*

### Procedura amministrativa: rimozione metodi MFA in Entra ID
<!-- graphify-evidence-id: ff7ba7848d80 -->

- **Source**: `Authenticator e Entra ID.txt`
- **Graph community**: 4

L’immagine mostra una schermata in cui viene richiesto il codice generato da Microsoft Authenticator, ma sul dispositivo nuovo non appare alcun account configurato. Questo scenario, unito all’errore 5

*Technology stack: to be enriched from source document.*

### Azure AD join (dispositivo aziendale)
<!-- graphify-evidence-id: 26dfdc75ca01 -->

- **Source**: `Authenticator e Entra ID.txt`
- **Graph community**: 4

L’immagine mostra una schermata in cui viene richiesto il codice generato da Microsoft Authenticator, ma sul dispositivo nuovo non appare alcun account configurato. Questo scenario, unito all’errore 5

*Technology stack: to be enriched from source document.*

### Macro VBA GatherLinksAndMakeClickableUniqueWithHeadingInline
<!-- graphify-evidence-id: 2b460b2866e7 -->

- **Source**: `Macro VBA per sistemare references.txt`
- **Graph community**: 12

Codice VBA Aggiornato 1. Apri il documento Word. 2. Premi Alt + F11 per aprire l'editor VBA. 3. Inserisci un nuovo modulo o modifica quello esistente: • Vai su Inserisci > Modulo se non hai già un m

*Technology stack: to be enriched from source document.*

### Word.Document.Hyperlinks
<!-- graphify-evidence-id: 2d3814700006 -->

- **Source**: `Macro VBA per sistemare references.txt`
- **Graph community**: 12

Codice VBA Aggiornato 1. Apri il documento Word. 2. Premi Alt + F11 per aprire l'editor VBA. 3. Inserisci un nuovo modulo o modifica quello esistente: • Vai su Inserisci > Modulo se non hai già un m

*Technology stack: to be enriched from source document.*

### Scripting.Dictionary (COM)
<!-- graphify-evidence-id: 98a61af35b75 -->

- **Source**: `Macro VBA per sistemare references.txt`
- **Graph community**: 12

' Dizionario per memorizzare i link già visti Set linkDict = CreateObject("Scripting.Dictionary") linkCount = 1 ' Loop attraverso tutti i link (dall'ultimo al primo per evitare problemi di spo

*Technology stack: to be enriched from source document.*

### Macro VBA EsportaTitoliInNuovoDoc
<!-- graphify-evidence-id: 0e974e8f4642 -->

- **Source**: `Macro VBA per titoli e sottotitoli.txt`
- **Graph community**: 12

Sub EsportaTitoliInNuovoDoc() Dim docOrigine As Document Dim docDestinazione As Document Dim par As Paragraph Dim livello As Long Dim testo As String Dim buffer As String Set d

*Technology stack: to be enriched from source document.*

### Paragraph.OutlineLevel (1-9 = titoli)
<!-- graphify-evidence-id: b0cf3da796ae -->

- **Source**: `Macro VBA per titoli e sottotitoli.txt`
- **Graph community**: 12

Sub EsportaTitoliInNuovoDoc() Dim docOrigine As Document Dim docDestinazione As Document Dim par As Paragraph Dim livello As Long Dim testo As String Dim buffer As String Set d

*Technology stack: to be enriched from source document.*

### Editor VBA Word (Alt+F11)
<!-- graphify-evidence-id: d54c1bc04508 -->

- **Source**: `Macro VBA per sistemare references.txt`
- **Graph community**: 12

Codice VBA Aggiornato 1. Apri il documento Word. 2. Premi Alt + F11 per aprire l'editor VBA. 3. Inserisci un nuovo modulo o modifica quello esistente: • Vai su Inserisci > Modulo se non hai già un m

*Technology stack: to be enriched from source document.*

### Script BAT log connessioni SSH
<!-- graphify-evidence-id: c9939196e1d3 -->

- **Source**: `file BAT.txt`
- **Graph community**: 25

@echo off setlocal :: Chiede all'utente l'indirizzo SSH set /p ssh_target=Inserisci host SSH (es. [EMAIL_1]): :: Log file (nella cartella utente) set log_file=%USERPROFILE%\ssh_connection_log.

*Technology stack: to be enriched from source document.*

### Percorsi di recupero MFA in Entra ID
<!-- graphify-evidence-id: 7428a61c1837 -->

- **Source**: `Authenticator e Entra ID.txt`

*Evidence text to be enriched from source document.*

*Technology stack: to be enriched from source document.*

### Bulk App Installation Flow
<!-- graphify-evidence-id: 53af65f3a4cc -->

- **Source**: `scripts`

*Evidence text to be enriched from source document.*

*Technology stack: to be enriched from source document.*

### Risposte audit autenticazione policy
<!-- graphify-evidence-id: 168f83a32989 -->

- **Source**: `Risposte-audit-autenticazione-policy.md`
- **Graph community**: 2

Question 29: Has the Sub-contractor defined, documented, and maintained a policy dealing with aspects such as authentication and user and password management (e.g., management of password length, comp

*Technology stack: to be enriched from source document.*

### Mail 23/03/2026 [EMAIL_5] -> asopranzi (centralino Vianova)
<!-- graphify-evidence-id: d0db79fdb2ba -->

- **Source**: `Ricerca Blocco Traffico in uscita per centralino_bf20e144.md`
- **Graph community**: 8

*Evidence text to be enriched from source document.*

*Technology stack: to be enriched from source document.*

### Microsoft 365 Exchange Online
<!-- graphify-evidence-id: 7d2760ffea7a -->

- **Source**: `Configurazione server IMAP in Odoo con mail Outlook.md`
- **Graph community**: 6

La mail [EMAIL_3] esiste su Exchange in Microsoft 365 Business, e se iniziamo a configurare un server di posta in arrivo in Odoo usando IMAP. Per questo la porta corretta è 993, non 587.

*Technology stack: to be enriched from source document.*

### Security Defaults tenant (blocca Basic Auth)
<!-- graphify-evidence-id: 8d99aece81cf -->

- **Source**: `Configurazione server IMAP in Odoo con mail Outlook.md`
- **Graph community**: 6

Per controllare se il Tenant blocca Basic Auth e in un tenant SENZA licenze Entra, l’unico che può farlo è Security Defaults. Se si va su “Ruoli assegnati” i ruoli sono: Serve il GLOBAL ADMINISTRATOR

*Technology stack: to be enriched from source document.*

### Client secret Azure Odoo Outlook Email
<!-- graphify-evidence-id: 4f8ed952f2f3 -->

- **Source**: `TREX.md`
- **Graph community**: 2

An error occurred when fetching the access token. AADSTS7000222: The provided client secret keys for app '8502941f-96e4-47a8-aa2d-cce8f91ff28d' are expired. Visit the Azure portal to create new keys f

*Technology stack: to be enriched from source document.*
