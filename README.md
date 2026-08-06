# Technical Skills Documentation

Public knowledge base documenting technical skills, capabilities, and operational responsibilities organized by domain.

Built with [MkDocs](https://www.mkdocs.org/) and the [Material](https://squidfunk.github.io/mkdocs-material/) theme.

**Live site**: https://alesop95.github.io/skills/

## Structure

Each Capability page follows a fixed schema:

1. **Overview** — what the Capability covers and why it matters
2. **Technologies & tools** — concrete stack with versions where relevant
3. **Responsibilities & operational scope** — operational scope and responsibilities
4. **Projects & evidence** — anonymized project entries demonstrating the Capability in practice

## Local preview

```bash
python -m venv .venv
source .venv/bin/activate   # Windows: .\.venv\Scripts\Activate.ps1
pip install -r requirements.txt
mkdocs serve
```

Then open http://127.0.0.1:8000/.

## Deploy

Push to `main` triggers an automatic build and deploy via GitHub Actions to GitHub Pages. See `.github/workflows/deploy.yml`.
