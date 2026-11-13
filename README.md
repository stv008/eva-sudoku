# Eva's Sudoku · Sudoku-ul Evei

A pastel Sudoku game made for Eva, in Romanian and English.

**Play:** https://stv008.github.io/eva-sudoku/

## What's in it

- **Three sizes:** *Primii pași* (4×4 with coloured shapes instead of numbers), *Exploratoare* (6×6) and *Campioană* (classic 9×9).
- **Three levels** per size: easy, medium and hard, worth 1, 2 or 3 stars.
- **Helpers, switchable on the start screen:** a hint button and red highlighting for wrong squares.
- **Family ladder:** each player picks their name before playing. The ladder ranks the fastest time for every size and level, plus the most stars collected. Each hint adds 15 seconds and each mistake 10, so a clean solve beats a fast but messy one.
- **Fresh puzzles every time.** Each one is generated in the browser and has exactly one solution.
- Works on phones, tablets and computers, in light and dark mode, and from the keyboard (digits, arrows, Backspace, H for a hint).

## Where scores are kept

On this website, players, stars and best times are saved **in the browser on each device** (`localStorage`). There are no accounts, no server and no tracking. Clearing the browser's site data resets the scores on that device.

The same page also runs as a Claude artifact. There it keeps one shared ladder for signed-in family members; outside Claude that part switches off automatically.

## Files

- `index.html` is the whole game: markup, styles and script in one file, with no build step and no dependencies. It uses two fonts from Google Fonts and falls back to system fonts without them.

## Publishing

GitHub Pages serves `index.html` from the `main` branch root (Settings → Pages → Deploy from a branch → `main` / `/ (root)`).
