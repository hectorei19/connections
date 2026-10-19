# Connections

Geography puzzle: 16 countries, four hidden groups of four. Pick four that share a category (a region, a flag, a language, a name...) and submit. Four mistakes and the game ends. Colours go from easiest to trickiest: yellow, green, blue, purple.

Part of a family of three games, each its own website: [Borderline](https://hectorei19.github.io/borderline/), [Connections](https://hectorei19.github.io/connections/) and [Top 10](https://hectorei19.github.io/top10/).

- Today's puzzle: the same for everyone, new at midnight CET (Spain), one try. Unlimited practice puzzles; a shared practice link (`?p=123`) opens the same puzzle.
- Results and stats are kept on the device (localStorage: `cx-daily`, `cx-free`, `cx-hist`).
- Every country fits its own group's category and none of the other three, so the puzzle has one solution. Independent countries only.

Files:
- `index.html` – the game.
- `data.js` – copy of Borderline's data: countries, flags, figures, categories (`CATS`) and their descriptions.
- `style.css` – Borderline's styles (colours, fonts, dark mode).
- `games.js` – the Games menu (top left). Each of the three projects has a copy: change it in one, copy it to the other two.
- `minigames.js` – helpers shared with Top 10 (a copy too).

Publishing a new version: change the `?v=` number after the four files in `index.html`, so phones load the new files.

Data sources and licences: see Credits in [Borderline](https://hectorei19.github.io/borderline/).
