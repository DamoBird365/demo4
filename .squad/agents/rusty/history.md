# Rusty — History

## Core Context

- **Project:** A glossy 5x5 Bingo card web app with tech buzzwords, deployed to GitHub Pages
- **Role:** Frontend Dev
- **Joined:** 2026-04-15T18:31:16.448Z

## Learnings

<!-- Append learnings below -->
- Marked tiles use greyed-out style (`#3a3a3a` gradient) instead of colorful cyan-purple gradient — user prefers muted/inactive look with readable text
- Tile click uses Y-axis spin animations (`spinIn`/`spinOut` keyframes with `perspective(600px) rotateY`) instead of the old `markPop` scale bounce
- `toggleTile()` manages animation classes (`spin-in`/`spin-out`) with `animationend` cleanup and reflow trick for re-triggering
- Key CSS locations: `.tile.marked` ~line 265, spin keyframes ~line 358, `toggleTile()` ~line 679
- FREE SPACE tile is excluded from toggle logic (early return on `FREE_INDEX`)
