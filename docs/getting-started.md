# Getting Started

Follow these steps to get the project running locally on your machine.

## Prerequisites

You will need the following installed before you begin:

- **Python 3.8+**
- **pip** (comes with Python)
- **Git**

## Installation

Clone the repository and create a virtual environment:

```bash
git clone https://github.com/MathiasDevelopes/mkdocs-oppgave.git
cd mkdocs-oppgave
python3 -m venv .venv
source .venv/bin/activate   # Windows: .venv\Scripts\activate
pip install -r requirements.txt
```

## Serve locally

```bash
.venv/bin/mkdocs serve
```

Open `http://localhost:8000` in your browser. The site reloads automatically whenever you save a file.

## Build

To generate the static site into the `site/` folder:

```bash
.venv/bin/mkdocs build
```

> [!WARNING] Don't commit `site/`
> The `site/` directory is git-ignored. GitHub Actions handles building and deploying automatically.

## Deploy manually

If you want to push to GitHub Pages without waiting for the Actions workflow:

```bash
.venv/bin/mkdocs gh-deploy --force
```

> [!INFO] First-time setup
> Make sure GitHub Pages is enabled in your **repository settings** and the source branch is set to `gh-pages`.
