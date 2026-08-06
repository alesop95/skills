# skills-repo - Claude Code instructions

Sei nella cartella **pubblica** `skills-repo` (GitHub: alesop95/skills). Tutto ciò che scrivi qui finisce online su `alesop95.github.io/skills/`.

Il motore privato che alimenta questo repo è `E:\lettore-doc`.

---

## Regola fondamentale

**Non scrivere mai dati sensibili** (nomi di clienti, codici progetto interni, indirizzi, importi specifici). I contenuti qui sono già stati anonimizzati da `export_to_taxonomy.py`. Se devi aggiungere testo manualmente, usa la stessa logica: aziende → "un'azienda del settore manifatturiero", nomi → ometti.

---

## Struttura della tassonomia

Ristrutturato il 2026-07-14: le Capability tecniche sono passate sotto `docs/technical/` (prima stavano alla radice di `docs/`) per lasciare spazio a una sezione separata `docs/soft/` per le soft skills, richiesta esplicitamente per alleggerire la sezione "Soft skills" del CV. La regola "non modificare la tabella Domain/Capability" di `docs/index.md` riguarda l'identita' e l'ordine dei Domain, non il path letterale dei link: quando le Capability si spostano, i link **vanno aggiornati**, altrimenti la build `--strict` fallisce (broken link). Gli URL tecnici pre-esistenti citati nel CV (`main.tex`) sono stati aggiornati in blocco per riflettere il nuovo prefisso `technical/`, quindi questo e' l'unico cambio di questo tipo previsto: non ripeterlo senza necessita', dato che ogni spostamento successivo richiederebbe un altro giro di aggiornamento dei link esterni.

```
docs/
├── index.md                     homepage - non modificare la tabella Domain/Capability
├── technical/                    Capability tecniche (schema fisso a 4 H2, vedi sotto)
│   ├── infrastructure/           Domain
│   │   ├── infrastructure-virtualization.md
│   │   ├── networking-engineering-security.md
│   │   └── backup-disaster-recovery.md
│   ├── security/
│   ├── cloud/
│   ├── software-engineering/
│   ├── data/
│   ├── it-operations/
│   └── management/
├── soft/                         Soft skills, testo libero raggruppato per tema, NON segue
│   └── index.md                  lo schema a 4 H2 e non ha <!-- graphify-evidence-id -->:
│                                  non fa parte della pipeline automatica di export_to_taxonomy.py.
└── graphify-out/
    └── graph.html               Knowledge Graph interattivo (non modificare)
```

---

## Schema fisso di ogni Capability page

Ogni `.md` ha **quattro H2 in ordine invariato**:

```markdown
## Overview
[prosa 3-6 righe - scritta manualmente, non sovrascrivere]

## Technologies & tools
[elenco con versioni - scritto manualmente, non sovrascrivere]

## Responsibilities & operational scope
[responsabilità - scritto manualmente, non sovrascrivere]

## Projects & evidence
[iniettato automaticamente da export_to_taxonomy.py]
[ogni entry è un H3 con commento HTML <!-- graphify-evidence-id: xxx -->]
[NON rimuovere i commenti HTML: sono l'ancora di idempotenza]
```

**Puoi modificare liberamente** Overview, Technologies & tools, Responsibilities. **Non rimuovere mai** i commenti `<!-- graphify-evidence-id: ... -->` in Projects & evidence.

---

## Aggiungere una nuova Capability manualmente

1. Creare `docs/technical/<domain>/<slug>.md` con lo schema a quattro H2
2. Aggiungere la riga al `mkdocs.yml` sotto il Domain corretto (dentro la voce "Technical"):
   ```yaml
   - Nome Capability: technical/<domain>/<slug>.md
   ```
3. `git add docs\technical\<domain>\<slug>.md mkdocs.yml`
4. `git commit -m "Add capability: <Nome Capability>"`
5. `git push` - deploy automatico in ~1 minuto

---

## Obsidian e Knowledge Graph

`docs/` aperta come vault in Obsidian permette di navigare la tassonomia in locale e di visualizzare il Knowledge Graph interattivo (`graphify-out/graph.html`) come tab nativo via plugin Embed HTML. Per plugin, uso ortogonale di graphify, flusso di rigenerazione e pubblicazione vedere `OBSIDIAN.md` nella root.

---

## Deploy

Ogni `git push` su `main` trigga GitHub Actions che esegue `mkdocs build --strict` e pubblica su Pages. Se la build fallisce (X rossa nelle Actions), controllare link rotti o riferimenti a file non esistenti.

```powershell
git add docs\
git commit -m "Messaggio descrittivo"
git push
```

---

## SSH e identità corretta

Questo repo è personale, non aziendale. Usare l'alias SSH personale:

```powershell
git remote -v   # verifica che punti a git@github-personal:alesop95/skills.git
```

Se il remote è sbagliato:
```powershell
git remote set-url origin git@github-personal:alesop95/skills.git
```

---

## URL stabili del sito

| Percorso file | URL pubblico |
|---------------|-------------|
| `docs/index.md` | `alesop95.github.io/skills/` |
| `docs/technical/infrastructure/networking-engineering-security.md` | `alesop95.github.io/skills/technical/infrastructure/networking-engineering-security/` |
| `docs/soft/index.md` | `alesop95.github.io/skills/soft/` |
| `docs/graphify-out/graph.html` | `alesop95.github.io/skills/graphify-out/graph.html` |

Nota: MkDocs Material con `use_directory_urls: true` (default) produce URL senza `.html`. Non cambiare mai il nome/percorso di un file già linkato nel CV **senza poi aggiornare anche il link lato CV**: la migrazione del 2026-07-14 (Capability tecniche spostate sotto `technical/`) e' stata fatta APPOSTA con l'ok esplicito dell'utente e con l'aggiornamento contestuale di tutti i link in `main.tex` - non e' un'eccezione alla regola, e' la procedura da seguire se in futuro serve spostare di nuovo qualcosa.

---

## Path locale e variabile d'ambiente

Il repo vive in locale a `E:\skills`. La variabile d'ambiente `LETTERDOC_SKILLS_REPO` deve puntare a questo path. Valore attuale: `E:\skills`.

Per verificare o aggiornare:

```powershell
[System.Environment]::GetEnvironmentVariable("LETTERDOC_SKILLS_REPO", "User")
# atteso: E:\skills

# Se necessario aggiornare:
[System.Environment]::SetEnvironmentVariable("LETTERDOC_SKILLS_REPO", "E:\skills", "User")
```
