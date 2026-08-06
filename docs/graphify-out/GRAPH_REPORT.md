# Graph Report - docs/  (2026-05-25)

## Corpus Check
- Corpus is ~6,876 words - fits in a single context window. You may not need a graph.

## Summary
- 141 nodes · 195 edges · 14 communities (12 shown, 2 thin omitted)
- Extraction: 80% EXTRACTED · 20% INFERRED · 0% AMBIGUOUS · INFERRED: 39 edges (avg confidence: 0.89)
- Token cost: 49,988 input · 21,423 output

## Community Hubs (Navigation)
- [[_COMMUNITY_Full-Stack Development & DevOps|Full-Stack Development & DevOps]]
- [[_COMMUNITY_Infrastructure & Virtualization|Infrastructure & Virtualization]]
- [[_COMMUNITY_LLMs & Workflow Automation|LLMs & Workflow Automation]]
- [[_COMMUNITY_Scripting & Data Processing|Scripting & Data Processing]]
- [[_COMMUNITY_Governance & Documentation|Governance & Documentation]]
- [[_COMMUNITY_Cybersecurity & Compliance|Cybersecurity & Compliance]]
- [[_COMMUNITY_Microsoft 365 & Business Apps|Microsoft 365 & Business Apps]]
- [[_COMMUNITY_Data Protection & Encryption|Data Protection & Encryption]]
- [[_COMMUNITY_Helpdesk & System Imaging|Helpdesk & System Imaging]]
- [[_COMMUNITY_Project Management|Project Management]]
- [[_COMMUNITY_UX & UI Design|UX & UI Design]]
- [[_COMMUNITY_Software License Management|Software License Management]]
- [[_COMMUNITY_Time & Attendance Systems|Time & Attendance Systems]]
- [[_COMMUNITY_Technical Hiring|Technical Hiring]]

## God Nodes (most connected - your core abstractions)
1. `Full-Stack Development & DevOps` - 18 edges
2. `LLMs & Generative AI` - 15 edges
3. `Ad-hoc Internal Development` - 15 edges
4. `Cybersecurity & IT Governance` - 12 edges
5. `Backup & Disaster Recovery` - 10 edges
6. `Data Protection & Cryptography` - 10 edges
7. `Cloud Platforms & Services` - 8 edges
8. `Zep + Ollama Self-Hosted Knowledge Management System` - 8 edges
9. `Technical Skills Documentation` - 7 edges
10. `Microsoft 365 Business` - 7 edges

## Surprising Connections (you probably didn't know these)
- `Clonezilla` --semantically_similar_to--> `Backup & Disaster Recovery`  [INFERRED] [semantically similar] docs/it-operations/formatting-machines-os.md → docs/infrastructure/backup-disaster-recovery.md
- `Business Continuity & Disaster Recovery Plans` --conceptually_related_to--> `Backup & Disaster Recovery`  [INFERRED] docs/management/quality-certification.md → docs/infrastructure/backup-disaster-recovery.md
- `GDPR` --conceptually_related_to--> `Data Protection & Cryptography`  [INFERRED] docs/security/cybersecurity-it-governance.md → docs/security/data-protection-cryptography.md
- `TypeScript` --semantically_similar_to--> `TypeScript`  [INFERRED] [semantically similar] docs/software-engineering/llms-generative-ai.md → docs/software-engineering/fullstack-development-devops.md
- `Technical Skills Documentation` --references--> `Data Management, Analytics & Reporting`  [EXTRACTED] docs/index.md → docs/data/data-management-analytics-reporting.md

## Hyperedges (group relationships)
- **Microsoft 365 Suite** — microsoft_365_business, microsoft_365_exchange, microsoft_365_sharepoint, microsoft_365_teams, microsoft_365_power_automate, microsoft_365_purview [EXTRACTED 1.00]
- **Backup Infrastructure** — backup_veeam, backup_qnap, backup_azure_backup, backup_ninjaone, infrastructure_proxmox [INFERRED 0.95]
- **Documentation Platforms** — documentation_itglue, documentation_obsidian, documentation_dokuwiki [EXTRACTED 1.00]
- **Vulnerability Scanning Tools** — openvas, nessus, vmware_vcenter_esxi [EXTRACTED 1.00]
- **Encryption Tools** — bitlocker, veracrypt, proton_drive, onedrive_personal_vault [EXTRACTED 1.00]
- **RAG Knowledge Management Stack** — zep, ollama, qdrant, typescript_llm, n8n_llm [EXTRACTED 1.00]

## Communities (14 total, 2 thin omitted)

### Community 0 - "Full-Stack Development & DevOps"
Cohesion: 0.09 Nodes (23): AI-Assisted Coding, CI/CD Pipelines, DevOps, Docker, Docker, ERP & Business Applications, Express, Full-Stack Development & DevOps (+15 more)

### Community 1 - "Infrastructure & Virtualization"
Cohesion: 0.16 Nodes (21): Microsoft Azure Backup, Backup & Disaster Recovery, NinjaOne Cloud Backup, QNAP NAS, Veeam Backup, Amazon AWS, Google Workspace, Microsoft Azure (+13 more)

### Community 2 - "LLMs & Workflow Automation"
Cohesion: 0.19 Nodes (17): Cheshire Cat, LLMs & Generative AI, Multi-LLM Orchestration, n8n, n8n, Ollama, Prompt Engineering, Qdrant (+9 more)

### Community 3 - "Scripting & Data Processing"
Cohesion: 0.21 Nodes (15): Ad-hoc Internal Development, Bash, Group Policy (GPO), NLP Processing, openpyxl, pandas, pdfplumber, PowerShell (+7 more)

### Community 4 - "Governance & Documentation"
Cohesion: 0.18 Nodes (14): DokuWiki, ITGlue, Obsidian, Entrepreneurship & Technical Leading, GDPR, IT Leadership Role Overview, ISO/IEC 27001, Leadership, Management & Cross-Cutting Responsibilities (+6 more)

### Community 5 - "Cybersecurity & Compliance"
Cohesion: 0.21 Nodes (12): Bitdefender GravityZone, CompTIA Security+, Cybersecurity & IT Governance, EDR Platform, ESET Business, GDPR, ISO/IEC 27001, Nessus (+4 more)

### Community 6 - "Microsoft 365 & Business Apps"
Cohesion: 0.20 Nodes (10): Microsoft 365 Billing Management, Italian SDI Electronic Invoicing, Google Cloud, Data Management, Analytics & Reporting, IT Administration & Billing, Microsoft 365 Business, Exchange Online, Power Automate (+2 more)

### Community 7 - "Data Protection & Encryption"
Cohesion: 0.39 Nodes (9): BitLocker, Data Protection & Cryptography, Encryption at Rest, KeePass XC, OneDrive Personal Vault, Password Management, Proton Drive, Vaultwarden (+1 more)

### Community 8 - "Helpdesk & System Imaging"
Cohesion: 0.50 Nodes (5): Advanced Helpdesk, Clonezilla, Formatting Machines & Operating Systems, Medicat USB, nLite Custom Windows Media

### Community 9 - "Project Management"
Cohesion: 0.60 Nodes (5): Product Management, Notion, OpenProject, Project Planning, Scheduling & Controlling, Trello

### Community 10 - "UX & UI Design"
Cohesion: 0.83 Nodes (4): IT Service Design & User Experience, Figma, Streamlit, UX & UI Design

### Community 11 - "Software License Management"
Cohesion: 1.00 Nodes (3): Apache Tomcat Migration (6 to 9), Ubuntu OS Migration (10.04 to 24.04), Software & License Management

## Knowledge Gaps
- **42 isolated node(s):** `Google Workspace`, `IPsec VPN`, `Medicat USB`, `Exchange Online`, `SharePoint Online` (+37 more) These have ≤1 connection - possible missing edges or undocumented components.
- **2 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `Ad-hoc Internal Development` connect `Scripting & Data Processing` to `Full-Stack Development & DevOps`?** _High betweenness centrality (0.062) - this node is a cross-community bridge._
- **Why does `LLMs & Generative AI` connect `LLMs & Workflow Automation` to `Scripting & Data Processing`?** _High betweenness centrality (0.056) - this node is a cross-community bridge._
- **Are the 2 inferred relationships involving `Ad-hoc Internal Development` (e.g. with `XLIFF` and `TMX`) actually correct?** _`Ad-hoc Internal Development` has 2 INFERRED edges - model-reasoned connections that need verification._
- **Are the 2 inferred relationships involving `Backup & Disaster Recovery` (e.g. with `Clonezilla` and `Business Continuity & Disaster Recovery Plans`) actually correct?** _`Backup & Disaster Recovery` has 2 INFERRED edges - model-reasoned connections that need verification._
- **What connects `Google Workspace`, `IPsec VPN`, `Medicat USB` to the rest of the system?** _43 weakly-connected nodes found - possible documentation gaps or missing edges._
- **Should `Full-Stack Development & DevOps` be split into smaller, more focused modules?** _Cohesion score 0.09486166007905138 - nodes in this community are weakly interconnected._