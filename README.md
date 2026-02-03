# Econometría e Inferencia Causal con ejemplos en Python

Libro en línea gratuito sobre econometría e inferencia causal con ejemplos prácticos en Python, construido con [Jupyter Book](https://jupyterbook.org).

**Autor:** Mario Alberto García Meza

**Sitio web:** [marionomics.github.io/econometria](https://marionomics.github.io/econometria/)

## Estructura del libro

1. **Introducción** — Historia de la inferencia causal, por qué los negocios necesitan econometría, e introducción a Python.
2. **Inferencia Causal** — Modelo de resultados potenciales y diseño de experimentos.
3. **Modelos** — Regresión lineal, series de tiempo, efectos fijos y diferencias en diferencias.
4. **Negocios** — Iteración con datos e investigación de mercados con inteligencia artificial.

## Requisitos

- Python 3.9+
- Jupyter Book (`pip install jupyter-book`)
- `ghp-import` para publicar en GitHub Pages (`pip install ghp-import`)

## Construir el libro

```bash
jupyter-book build .
```

El HTML generado estará en `_build/html/`.

## Publicar en GitHub Pages

```bash
ghp-import -n -p -f _build/html
```

## Más información

Visita [marionomics.com](https://www.marionomics.com) para más contenido sobre econometría y ciencia de datos.
