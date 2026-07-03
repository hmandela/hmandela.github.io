# hmandela.com

Personal website of Mandela HOUNGNIBO, built with [Quarto](https://quarto.org/).

## Local preview

```bash
quarto preview
```

## Add a blog post

Create `blog/YYYY-MM-DD-short-name/en/index.qmd` (and optionally `fr/index.qmd` for the French version). Listings, feeds and the homepage pick it up automatically.

## Add a talk

Copy `talks/_template/` to `talks/YYYY-MM-short-name/` and edit `index.qmd`.

## Deploy

Pushing to `main` triggers `.github/workflows/publish.yml`, which renders the site and publishes it to the `gh-pages` branch (GitHub Pages). Computational output is frozen (`freeze: auto`), so CI does not need Python/R — render posts locally and commit the `_freeze/` directory.
