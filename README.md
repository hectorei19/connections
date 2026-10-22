# Connections (Geomingo)

Part of [Geomingo](https://hectorei19.github.io/geo-games/). Colours, fonts, Mingo, the header and the result window come from `../geo-games/brand/` (repository hectorei19/geo-games); `games.js`, `minigames.js` and `style.css` are shared copies with Top 10 and Silhouette.

Geography puzzle: 16 countries, four hidden groups of four. Pick four that share a category (a region, a flag, a language, a name...) and submit. Four mistakes and the game ends. Colours go from easiest to trickiest: yellow, green, blue, purple.

Part of [Geomingo](https://hectorei19.github.io/geo-games/), daily geography games, each its own website: [Countries](https://hectorei19.github.io/country-grid/), [Connections](https://hectorei19.github.io/connections/) and [Top 10](https://hectorei19.github.io/top10/).

- The page opens on today's puzzle, as Countries (formerly Country Grid) opens on today's grid: tap a country to start.
- Today's puzzle: the same for everyone, new at midnight CET (Spain), one try. Solo: unlimited practice puzzles; a shared practice link (`?p=123`) opens the same puzzle.
- With friends: online rooms for 2 to 8 players, each on their own phone, all playing the same puzzle at the same time with everyone's progress shown live. Solved first, then fewer mistakes, then faster. A room link (`?room=ABCD`) joins that room. Rooms live in Countries' Firebase Realtime Database under `rooms/ABCD` (tagged `game: 'connections'`), so Countries' database rules already cover them.
- Results and stats are kept on the device (localStorage: `cx-daily`, `cx-free`, `cx-hist`; for rooms `cx-pid`, `cx-name`, `cx-room`, `cx-online`).
- Every country fits its own group's category and none of the other three, so the puzzle has one solution. Independent countries only.

Files:
- `index.html` – the game.
- `data.js` – copy of Countries' data: countries, flags, figures, categories (`CATS`) and their descriptions.
- `style.css` – Countries' styles (colours, fonts, dark mode).
- `games.js` – the Games menu (top left). Each of the three projects has a copy: change it in one, copy it to the other two.
- `minigames.js` – helpers shared with Top 10 (a copy too).
- `firebase-config.js` – Countries' Firebase web config (a copy), for With friends.

Publishing a new version: change the `?v=` number after the files in `index.html`, so phones load the new files.

Data sources and licences: see Credits in [Countries](https://hectorei19.github.io/country-grid/).
