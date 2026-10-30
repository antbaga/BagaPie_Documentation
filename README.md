# BagaPie documentation

User documentation for BagaPie 11 (11.0.11). MkDocs + Read the Docs theme, published with GitHub Pages.

Site: https://antbaga.github.io/BagaPie_Documentation/

## Edit locally

Edit the Markdown files in `docs/`. Navigation is in `mkdocs.yml`.

```powershell
python -m pip install -r requirements.txt
python -m mkdocs serve
```

Open http://127.0.0.1:8000. Changes reload automatically.

## Publish

```powershell
python -m mkdocs build --strict
git add .
git commit -m "Update documentation"
git push origin main
```

GitHub Actions builds and publishes to `gh-pages`. In the repository's **Settings > Pages**, the source is **Deploy from a branch**, branch **gh-pages**, folder **/ (root)**.

Do not edit generated files in `site/` or on `gh-pages`.

## Content

Document implemented behavior only. Sources for this edition: the add-on code (11.0.11 manifest, operators, panel and preferences) and the BagaPie 11 tutorial playlist. When updating, check the code: the tutorials may lag behind the current defaults.

GIFs are step sequences taken from the tutorial videos; see `GIF-SOURCES.md`.
