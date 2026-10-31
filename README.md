# Kopi Guide

Documentation site built with [MkDocs](https://www.mkdocs.org/) and the [Material](https://squidfunk.github.io/mkdocs-material/) theme.

## Working locally

Requires Python 3.9 or later.

```bash
python -m venv .venv
.venv/bin/pip install -r requirements.txt      # Windows: .venv\Scripts\pip install -r requirements.txt
.venv/bin/mkdocs serve                          # live-reloading preview
.venv/bin/mkdocs build --strict                 # production build into site/
```

Pages are Markdown files in `docs/`; pictures go in `docs/img/` and are linked relative to the page.

## Deploying

Publish changes with:

```bash
mkdocs gh-deploy
```

It builds the site and pushes it to the `gh-pages` branch (created on the first run). After the first deploy, check that **Settings → Pages** shows **Deploy from a branch**, branch `gh-pages`, folder `/ (root)`.
