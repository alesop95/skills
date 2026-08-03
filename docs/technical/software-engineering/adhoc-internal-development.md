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
