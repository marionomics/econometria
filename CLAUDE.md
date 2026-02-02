# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a free, open-source Spanish-language textbook on econometrics and causal inference with Python examples ("Econometría e Inferencia Causal con ejemplos en Python"), built with **Jupyter Book**. Author: Mario Alberto García Meza.

## Build Commands

```bash
# Build the book (from repo root)
jupyter-book build econometria/

# Clean build artifacts before rebuilding
jupyter-book clean econometria/
```

The HTML output goes to `econometria/_build/html/`. The config sets `execute_notebooks: force`, so all notebooks are re-executed on every build.

## Dependencies

```bash
pip install -r econometria/requirements.txt
```

Core dependencies: `jupyter-book`, `matplotlib`, `numpy`.

## Architecture

- `econometria/_config.yml` — Jupyter Book configuration (title, execution settings, repository links, LaTeX config, bibliography)
- `econometria/_toc.yml` — Table of contents defining book structure and chapter order
- `econometria/intro.md` — Book landing page
- `econometria/references.bib` — BibTeX bibliography
- `econometria/chapters/` — Chapter content organized by part:
  - `I-Introduccion/` — Part I chapters (Python for econometrics, potential outcomes)
  - `II-Recursos/` — Part II (exercises)
- `econometria/figures/` — Images referenced by chapters
- `econometria/_build/` — Generated output (not committed)

## Content Conventions

- All prose is written in **Spanish**
- Chapters are Jupyter notebooks (`.ipynb`) with sequential numeric prefixes (e.g., `01-`, `02-`, `03-`)
- New chapters must be registered in `_toc.yml` to appear in the book
- The book uses BibTeX for citations via `references.bib`
- Repository is configured for GitHub issues button and repository link button in the HTML output
