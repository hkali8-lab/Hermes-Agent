# Hermes-Agent

Public site for the `hkali8-lab/Hermes-Agent` project, deployed to GitHub Pages.

## What this repo contains

- `index.html` — a self-contained static landing page (no build step, no external deps).
- `.github/workflows/deploy-pages.yml` — GitHub Actions workflow that builds and
  deploys the site to GitHub Pages on every push to `main`, and on demand.
- `README.md` — this file.

## Deployment

This repository is a **GitHub Pages (custom workflow)** site. The workflow
uploads the repo root as the Pages artifact and deploys it via the official
`actions/deploy-pages`. Pages is configured with `build_type: workflow` and
source `main:/`.

- Live URL: `https://hkali8-lab.github.io/Hermes-Agent/`
- Runs: GitHub → **Actions** tab

Deploy manually any time: Actions → “Deploy to GitHub Pages” → **Run workflow**.

## Local development

Open `index.html` directly in a browser, or:

```bash
python3 -m http.server 8080
# → http://localhost:8080
```
