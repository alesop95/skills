# Obsidian — skills

Questo file documenta come aprire e usare il vault Obsidian su `docs/` e come
generare o aggiornare il Knowledge Graph interattivo con graphify. Va letto
insieme a `CLAUDE.md`.

---

## Cos'e' il vault

`docs/` e' la root dei contenuti MkDocs del sito pubblico `alesop95.github.io/skills/`.
Aperta come vault in Obsidian diventa uno strumento di navigazione locale della
tassonomia: si leggono e modificano le Capability page, si naviga il grafo delle
note via wiki-link, e si visualizza il Knowledge Graph interattivo generato da
graphify senza aprire il browser.

La cartella `.obsidian/` e' gitignored (`E:\skills\.gitignore`): la configurazione
Obsidian resta locale e non viene mai pubblicata.

---

## Aprire il vault

File -> Open folder as vault -> `E:\skills\docs\`

Il vault e' gia' configurato (`.obsidian/` presente con plugin attivi). Non serve
nessun setup aggiuntivo.

---

## Plugin attivi

*BRAT* (Beta Reviewer's Auto-update Tool): gestore dei plugin beta. Attivo.

*3D Graph* (da `Apoo711/obsidian-3d-graph`): grafo tridimensionale delle note.
Utile per visualizzare le relazioni tra le Capability page e i Domain. Si apre
dall'icona in barra laterale o con Ctrl+P -> Open 3D Graph.

*Embed HTML* (autore mnaoumov): apre i file `.html` come tab nativi. Il file
`graphify-out/graph.html` si apre con un click nel file explorer di Obsidian,
senza sintassi speciali. E' il modo principale per visualizzare il Knowledge Graph
in locale.

---

## Il Knowledge Graph: uso ortogonale di graphify

graphify viene usato su questo vault in modo ortogonale rispetto all'uso su
documenti sorgente: invece di estrarre conoscenza da documentazione privata, legge
le Capability page Markdown di `docs/` e costruisce un grafo delle relazioni
semantiche tra skill — quali Capability condividono tecnologie, responsabilita' o
approcci metodologici.

Il grafo risultante (`docs/graphify-out/graph.html`) e' un asset statico del sito
MkDocs e viene pubblicato all'URL:

```
https://alesop95.github.io/skills/graphify-out/graph.html
```

### Rigenerare il grafo

Aprire Claude Code nella root `E:\skills` e lanciare:

```
/graphify docs/
```

graphify legge le Capability page, costruisce il grafo, scrive `graph.html` in
`docs/graphify-out/`. Obsidian mostra immediatamente la versione aggiornata
(Embed HTML ricarica il tab al cambio file). Per pubblicarlo:

```powershell
git add docs\graphify-out\graph.html
git commit -m "Aggiornato Knowledge Graph"
git push
```

Il deploy su GitHub Pages avviene in circa un minuto tramite GitHub Actions.

### Cosa non versionare

Il `.gitignore` di `E:\skills` esclude i file intermedi di graphify:

```
docs/graphify-out/.graphify_*
docs/graphify-out/converted/
docs/graphify-out/cache/
docs/graphify-out/*.json
docs/graphify-out/cost.json
docs/graphify-out/manifest.json
```

Solo `graph.html` viene committato e pubblicato.

---

## Struttura del vault

```
docs/
├── index.md                     homepage della tassonomia
├── infrastructure/              Domain con le Capability page
├── security/
├── cloud/
├── software-engineering/
├── data/
├── it-operations/
├── management/
└── graphify-out/
    └── graph.html               Knowledge Graph interattivo (aprire con Embed HTML)
```

Ogni Capability page ha quattro sezioni H2 in ordine invariato: Overview,
Technologies & tools, Responsibilities & operational scope, Projects & evidence.
Le prime tre si modificano liberamente. La quarta e' gestita da
`export_to_taxonomy.py` via commenti HTML di idempotenza: non rimuovere mai quei
commenti.

---

## Server MCP obsidian-vaults

Il server MCP `obsidian-vaults` (configurato a livello di account in
`~/.claude-accountN/mcp.json` e nella app claude.ai desktop) espone anche `docs/`
come filesystem accessibile all'agente. Questo permette di lavorare sulle Capability
page senza essere necessariamente nel CLI locale.

Casi d'uso rilevanti per questo vault:

Aggiornare una Capability page da una sessione claude.ai (account1) senza aprire
Claude Code CLI — Claude legge la pagina corrente via MCP e la riscrive con
`write_file` direttamente in `docs/`, da qualsiasi client Claude con il server attivo.

Ricerca trasversale tra pagine — `search_files` su tutta `docs/` per verificare
coerenza, trovare duplicati o individuare dove una tecnologia e' gia' citata prima
di aggiungere una nuova Capability.

graphify da claude.ai — in prospettiva, lanciare `/graphify docs/` da una sessione
claude.ai invece che dal CLI locale: il server MCP legge le Capability page e scrive
il grafo in `docs/graphify-out/`. (Richiede che la skill graphify sia disponibile
nella sessione.)

Il server e' attivo in tutte le sessioni Claude Code (account1 e account2) e nella
app claude.ai desktop. E' un accesso parallelo allo stesso filesystem: le modifiche
scritte via MCP sono immediatamente visibili in Obsidian e nel repo locale.

---

## Flusso completo

```
E:\lettore-doc (pipeline privata)
    |
    v
export_to_taxonomy.py --apply
    |
    v
E:\skills/docs/  <-- questo vault
    |
    +---> [navigazione locale in Obsidian]
    |
    +---> /graphify docs/  (uso ortogonale: grafo delle sole skill)
    |         |
    |         v
    |     docs/graphify-out/graph.html
    |         |
    |         +---> [visualizzazione in Obsidian via Embed HTML]
    |         |
    |         +---> git push -> GitHub Actions -> alesop95.github.io/skills/graphify-out/graph.html
    |
    +---> mkdocs build (via GitHub Actions su ogni push)
              |
              v
         alesop95.github.io/skills/
```
