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

Player profiles and the leaderboard live in `localStorage`, so progress is per-browser/per-device. Keys: `mq:player:<NAME>`, `mq:leaderboard`.
