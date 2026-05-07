# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Commands

All MkDocs commands must use the local venv:

```bash
# Serve locally with live reload
.venv/bin/mkdocs serve

# Build static site into site/
.venv/bin/mkdocs build

# Deploy directly to gh-pages branch (manual deploy)
.venv/bin/mkdocs gh-deploy --force

# Install/update dependencies
.venv/bin/pip install -r requirements.txt
```

## Architecture

This is a static documentation site. There is no application code — all content is Markdown.

- **`mkdocs.yml`** — single source of truth for site config: theme, nav, Markdown extensions, and `site_url`. The `nav:` block controls page order and sidebar structure.
- **`docs/`** — all Markdown content. Files map 1-to-1 to URLs (`docs/guide/overview.md` → `/guide/overview/`).
- **`.github/workflows/deploy.yml`** — on every push to `main`, installs `mkdocs-material` and runs `mkdocs gh-deploy --force`, which builds and force-pushes the `site/` output to the `gh-pages` branch.
- **`site/`** — generated output, git-ignored, never edit manually.

## Deployment

GitHub Pages must be configured in the repo settings to serve from the `gh-pages` branch. The live site URL is `https://MathiasDevelopes.github.io/mkdocs-oppgave/`.

## Adding content

Add a new `.md` file under `docs/` and register it in the `nav:` section of `mkdocs.yml`. MkDocs will 404 on any page not listed in `nav`.
