# About

This documentation site was created as a **school assignment** to explore and demonstrate [MkDocs Material](https://squidfunk.github.io/mkdocs-material/) — a powerful documentation framework built on top of MkDocs.

## Goals

The assignment covers:

1. Setting up a local MkDocs Material project
2. Customising the theme (colours, fonts, navigation)
3. Writing structured documentation in Markdown
4. Automating deployment to GitHub Pages via GitHub Actions

## Tech stack

| Tool              | Role                                    |
|-------------------|-----------------------------------------|
| MkDocs            | Static site generator                   |
| MkDocs Material   | Theme and UI components                 |
| mkdocs-callouts   | Obsidian-style callout syntax           |
| GitHub Actions    | CI/CD — deploys on every push to `main` |
| GitHub Pages      | Free static hosting                     |

## Deployment pipeline

Every push to the `main` branch triggers the workflow in `.github/workflows/deploy.yml`. It:

1. Installs `mkdocs-material` and dependencies
2. Runs `mkdocs gh-deploy --force`
3. Force-pushes the built `site/` output to the `gh-pages` branch
4. GitHub Pages serves that branch at the public URL

> [!SUCCESS] Live site
> **[MathiasDevelopes.github.io/mkdocs-oppgave](https://MathiasDevelopes.github.io/mkdocs-oppgave/)**
