# Ad-hoc Internal Development

## Overview

Custom in-house development of utilities, automation scripts, and small
internal applications to support operational and project-management
workflows. Spans Bash, PowerShell, and Python scripting for system
automation, NLP/XML processing for translation-industry workflows, and
desktop GUI development for distribution and onboarding tooling.

## Technologies & tools

- **Python** — primary scripting language; libraries include `pdfplumber`,
  `openpyxl`, `pandas`, `spaCy`
- **Bash** — Ubuntu cleanup, mailer setup, and system automation
- **PowerShell** — endpoint scripting embedded in NinjaOne RMM
- **Qt Designer** — desktop GUI development for internal Windows tools
- **Regex** — XML/TMX/XLIFF content manipulation
- Group Policy (GPO) for Windows-domain user lifecycle automation

## Responsibilities & operational scope

### General automation and scripting

- Bash, PowerShell, and Python scripting for system automation
- Bash scripts for Ubuntu cleanup and mailer environment setup
- PowerShell scripts deployed via NinjaOne RMM for endpoint automation
- Software plugin integration
- Development of internal applications to facilitate project-management
  work (e.g. Python+Qt Designer GUI tool for software distribution on
  Windows)

### Python local scripting utilities

- Character-count-per-line analysis on `.txt` files
- Text extraction from PDF files to `.txt` (using `pdfplumber`)
- Bulk conversion of `.xlsx` files in a folder to comma-separated `.txt`
  files (using `openpyxl`)
- Validation that strings in a file do not exceed a defined maximum
  length
- Text extraction from `.docx` and `.xlsx` files to `.txt`
- Splitting an Excel workbook into multiple files, one per sheet
- Preparation of files for translators in a structured, automated way,
  starting from a complex multilingual Excel
- Excel preprocessing and multi-file splitting via `pandas`

### NLP and XML scripting

- Extraction of common single words, acronyms, bigrams, and trigrams
  from `.txt` files via `spaCy`, generating `.json` and `.txt`
  glossaries with relative and absolute frequency thresholds
- Reduction of a Translation Memory (TMX) by retaining only a
  configurable percentage of translation units
- Management and manipulation of hidden XML content via regex
- Encoding and restoration of text content enclosed in XML tags
- Extraction of the "skeleton" of a translated XML file using a
  multi-line block manager, and reconstruction of the translated XML
  file by reinserting translated sentences in place of numeric
  placeholders in the skeleton

### Cross-cutting utilities

- Group Policy (GPO) management for Windows-domain user lifecycle
- Complete user onboarding and offboarding automation
- Advanced JSON parsing
- Custom Trados GroupShare TM plugin automation inside Windows

## Projects & evidence

### net user command
<!-- graphify-evidence-id: 832ee892620e -->

- **Source**: `1. L'account che si crea è un account Admin all'inizio poi si crea un account locale.txt`
- **Graph community**: 5

net user NOMEUTENTE /add dove "NOMEUTENTE" è self-explicative come parametro. Per impostare una password per l'account appena creato: net user NOMEUTENTE PASSWORD

*Technology stack: to be enriched from source document.*

### [HOSTNAME_13] VM ([IP_7], desktop remoto PM/DTP)
<!-- graphify-evidence-id: fbcdd76c85b8 -->

- **Source**: `ARCHITETTURA [HOSTNAME_56] 20052026_b5a58014.md`
- **Graph community**: 6

Una volta selezionata la cartella, fare clic su Finish e quindi su Close per completare l’operazione. Il progetto aperto da Groupshare è ora visualizzato nella lista di progetti disponibili. Il PM, es

*Technology stack: to be enriched from source document.*

### Cleanup PowerShell Remove-Item -Recurse -Force
<!-- graphify-evidence-id: 4e29772f665e -->

- **Source**: `Perche inoltre ho tre cartelle di i.txt`
- **Graph community**: 20

*Evidence text to be enriched from source document.*

*Technology stack: to be enriched from source document.*

### Pivot: dove sta il cestino in Windows 11 (Icone desktop, shell:RecycleBinFolder)
<!-- graphify-evidence-id: 8ba9decb61d2 -->

- **Source**: `screenshot_16.png`
- **Graph community**: 6

*Evidence text to be enriched from source document.*

*Technology stack: to be enriched from source document.*

### Introduzione PowerShell ISE breakpoints (Set-PSBreakpoint)
<!-- graphify-evidence-id: 42fb69415c8e -->

- **Source**: `screenshot_19.png`
- **Graph community**: 6

*Evidence text to be enriched from source document.*

*Technology stack: to be enriched from source document.*

### Verifica GUI Proprieta Cestino: 10240 MB su tutti e 4 i volumi
<!-- graphify-evidence-id: 42bb0aebc23a -->

- **Source**: `Script powershell per limitazione spazio cestino per utenti`

*Evidence text to be enriched from source document.*

*Technology stack: to be enriched from source document.*

### Deep dive su variabili PowerShell e SID
<!-- graphify-evidence-id: fb4d966a8895 -->

- **Source**: `screenshot_23.png`

*Evidence text to be enriched from source document.*

*Technology stack: to be enriched from source document.*

### gpedit.msc (Group Policy Editor)
<!-- graphify-evidence-id: faae9fb23d17 -->

- **Source**: `Configurazione-autenticazione-Windows.md`
- **Graph community**: 2

Cliccare su Applica e chiudere. Per configurare la scadenza e le caratteristiche della password cliccare WIN+R, digitare gpedit.msc Seguire “Configurazione computer->Impostazioni di Windows->Impostazi

*Technology stack: to be enriched from source document.*

### Sub-organization LANGUAGE RESOURCES
<!-- graphify-evidence-id: dab647d4ed97 -->

- **Source**: `2022-11-07_Creazione di una memoria su Groupshare 2020.md`
- **Graph community**: 2

LANGUAGE RESOURCES Questa cartella contiene le sub-organization in cui sono create le TM settoriali (es. FINANCE, GDPR, PHARMA), quelle usate per tradurre il materiale aziendale interno (INTRAWELT) e

*Technology stack: to be enriched from source document.*

### Language Processing Rules e Field Template
<!-- graphify-evidence-id: 486028fbff4a -->

- **Source**: `2022-11-07_Creazione di una memoria su Groupshare 2020.md`
- **Graph community**: 2

Selezionare la lingua source e quella target, quindi modificare se necessario Language Processing Rules e Field Template. Negli Advanced Settings, generalmente la configurazione più efficace è quella

*Technology stack: to be enriched from source document.*

### Gestione credenziali Windows
<!-- graphify-evidence-id: 5cb0019b8b15 -->

- **Source**: `gestione credenziali windows.md`
- **Graph community**: 3

*Evidence text to be enriched from source document.*

*Technology stack: to be enriched from source document.*

### Trados Studio (CAT tool)
<!-- graphify-evidence-id: 16f742e25db3 -->

- **Source**: `[HOSTNAME_8].md`
- **Graph community**: 3

Qui https://appstore.rws.com/Plugin/263 c'è un toolkit relativo a Trados Studio 2024. Facendo clic su Download ti fa arrivare a github: https://github.com/RWS/Sdl-studio-powershell-toolkit.

*Technology stack: to be enriched from source document.*

### Formato SDLXLIFF (bilingue basato su XLIFF/XML)
<!-- graphify-evidence-id: d43bd79d859b -->

- **Source**: `[HOSTNAME_8].md`
- **Graph community**: 5

La software house era sdl (ora rvs) ma il formato proprietario è rimasto lo stesso, è un formato basato su xliff, derivato da XML che è preparato per essere bilingue. Aprendo la cartella di progetto d

*Technology stack: to be enriched from source document.*

### Trados Accelerate (cloud collaboration)
<!-- graphify-evidence-id: bc573dbfe3cd -->

- **Source**: `[HOSTNAME_8].md`
- **Graph community**: 3

Trados Accelerate: architettura cloud-based per la collaborazione su progetti pubblicati che si interfaccia anch’essa con l’applicazione desktop pro dei PM e le applicazioni desktop freelancer dei lin

*Technology stack: to be enriched from source document.*

### Trados GroupShare (on-premise collaboration)
<!-- graphify-evidence-id: a799f8f30526 -->

- **Source**: `[HOSTNAME_8].md`
- **Graph community**: 3

Trados Groupshare: architettura server on-premise per la collaborazione su progetti pubblicati che si interfaccia con l’applicazione desktop pro dei PM e le applicazioni desktop freelancer dei linguis

*Technology stack: to be enriched from source document.*

### [HOSTNAME_1] server (LAN [IP_4] / WAN [IP_5])
<!-- graphify-evidence-id: 417982234241 -->

- **Source**: `[HOSTNAME_8].md`
- **Graph community**: 3

RWS Trados Studio: applicazione desktop con licenza pro appoggiata su license server. Trados Groupshare: architettura server on-premise per la collaborazione su progetti pubblicati che si interfaccia

*Technology stack: to be enriched from source document.*

### GroupShare API PowerShell Toolkit
<!-- graphify-evidence-id: fd3f529653b0 -->

- **Source**: `[HOSTNAME_8].md`
- **Graph community**: 3

Qui https://appstore.rws.com/Plugin/268 c'è un toolkit che dovrebbe consentire di automatizzare alcune operazioni in Groupshare, fare manutenzione sulle TM, ecc… Facendo clic su Download ti fa arrivar

*Technology stack: to be enriched from source document.*

### Trados Accelerate Language Cloud PowerShell Toolkit
<!-- graphify-evidence-id: c894d399e2bf -->

- **Source**: `[HOSTNAME_8].md`
- **Graph community**: 3

Qui https://appstore.rws.com/Plugin/283, ma fronte Trados Accelerate. Facendo clic su Download ti fa arrivare a github: https://github.com/RWS/language-cloud-powershell-toolkit. Trados Studio 2

*Technology stack: to be enriched from source document.*

### Trados Studio 2024 PowerShell Toolkit
<!-- graphify-evidence-id: 7efd310def4d -->

- **Source**: `[HOSTNAME_8].md`
- **Graph community**: 3

Qui https://appstore.rws.com/Plugin/263 c'è un toolkit relativo a Trados Studio 2024. Facendo clic su Download ti fa arrivare a github: https://github.com/RWS/Sdl-studio-powershell-toolkit.

*Technology stack: to be enriched from source document.*

### Configurazione FileType (XML, testo delimitato con regex, embedded content)
<!-- graphify-evidence-id: eb921a2a4a0a -->

- **Source**: `[HOSTNAME_8].md`
- **Graph community**: 3

casellina filetype > seleziona il filetype corrispondente (Microsoft Word/Excel 2007-2019) > Embedded content > flag su 'Enable embedded content processing' e su 'Extract in all paragraphs' > Add > ne

*Technology stack: to be enriched from source document.*

### PowerShell Connect-ExchangeOnline
<!-- graphify-evidence-id: 09105cdf765d -->

- **Source**: `Configurazione server IMAP in Odoo con mail Outlook.md`
- **Graph community**: 6

PS C:\Users\Utente> Connect-ExchangeOnline Set-Mailbox [EMAIL_3] -Type Regular E:

*Technology stack: to be enriched from source document.*
