# CLAUDE.md

## Project overview

This is a Jupyter Book project for an online econometrics textbook: "Econometría e Inferencia Causal con ejemplos en Python" by Mario Alberto García Meza. The book is written in Spanish and published via GitHub Pages.

## Repository structure

- `_config.yml` — Jupyter Book configuration
- `_toc.yml` — Table of contents defining book structure
- `intro.md` — Book landing page
- `references.bib` — Bibliography in BibTeX format
- `chapters/` — Book content organized in parts:
  - `I-Introduccion/` — Chapters 00-02 (causal inference intro, business motivation, Python intro)
  - `II-Inferencia-Causal/` — Chapters 03-04 (potential outcomes, experiments)
  - `III-Modelos/` — Chapters 05-08 (regression, time series, fixed effects, diff-in-diff)
  - `IV-Negocios/` — Chapters 09-10 (iteration, market research with AI)
- `figures/` — Images and diagrams used in chapters
- `_build/` — Generated output (not committed)

## Build commands

```bash
# Build the book
jupyter-book build .

# Publish to GitHub Pages
ghp-import -n -p -f _build/html
```

## Key details

- Language: Spanish
- Notebooks are re-executed on every build (`execute_notebooks: force` in `_config.yml`)
- Remote: `git@github.com:marionomics/econometria.git`
- GitHub Pages URL: https://marionomics.github.io/econometria/
- Main branch: `main`
- GitHub Pages branch: `gh-pages`
