# Squad Decisions

## Active Decisions

### Tile Spin + Greyed-Out Marked Style

**Author:** Rusty (Frontend Dev)  
**Date:** 2025-07-15  
**Status:** Implemented  

Visual language shift for marked tiles: replaced `markPop` scale animation with `spinIn`/`spinOut` Y-axis 360° rotations using CSS perspective. Marked tiles now display dark grey (`#3a3a3a`) background with readable text instead of colorful gradient. Animation classes managed in `toggleTile()` with `animationend` listener cleanup. Unmarking reverses spin direction. No impact on FREE SPACE tile or win-line styling.

### GitHub Pages Deployment

**Author:** Linus (DevOps)  
**Date:** 2025-07-15  
**Status:** Implemented  

Deploy Tech Bingo via GitHub Pages using Actions workflow approach. Workflow file: `.github/workflows/deploy-pages.yml`. Source: `main` branch root. Live URL: https://damobird365.github.io/demo4/. Actions workflow provides better control over deployment pipeline and is GitHub's recommended path forward.

## Governance

- All meaningful changes require team consensus
- Document architectural decisions here
- Keep history focused on work, decisions focused on direction
