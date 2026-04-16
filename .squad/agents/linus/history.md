# Linus — History

## Core Context

- **Project:** A glossy 5x5 Bingo card web app with tech buzzwords, deployed to GitHub Pages
- **Role:** DevOps
- **Joined:** 2026-04-15T18:31:16.455Z

## Learnings

<!-- Append learnings below -->
- GitHub Pages enabled on `DamoBird365/demo4` using Actions workflow deployment (`build_type: workflow`)
- Deployment workflow: `.github/workflows/deploy-pages.yml` — uses `actions/deploy-pages@v4`
- Pages source: `main` branch, root `/` directory
- Live URL: https://damobird365.github.io/demo4/
- Single static `index.html` — no build step needed, uploads entire repo root as artifact
- GitHub Actions disabled for this user account — workflow-based Pages deploy (`build_type: workflow`) will not trigger
- Switched Pages to legacy deployment: `build_type: legacy`, source branch `gh-pages`, path `/`
- Created orphan `gh-pages` branch containing only `index.html` (no .squad/, .github/, etc.)
- API call to switch: `'{"source":"gh-pages","build_type":"legacy"}' | gh api repos/DamoBird365/demo4/pages -X PUT --input -`
- Legacy deploy accepted sources: gh-pages, master, master /docs — the API `source` field is a flat string, not a JSON object
- `.github/workflows/deploy-pages.yml` left in place on main — harmless since Actions won't run
