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
