# math-quest

A single-file HTML math practice game. Multiplication, distribution, and fractions, dressed up as a retro arcade.

**Play it:** https://manugarg.github.io/math-quest/

## Run locally

It's one file, no build step. Either:

```sh
open index.html       # macOS
xdg-open index.html   # Linux
```

…or just double-click `index.html`.

## Storage

Player profiles live in `localStorage` (per-browser/per-device), keyed `mq:player:<NAME>`.

The leaderboard is shared globally via Firebase Firestore (project `fun-tools-mg`, collection `leaderboard`, doc id = URL-encoded player name). A copy of the most recent fetch is cached in `localStorage` under `mq:leaderboard` so the Hall of Fame still renders when offline.
