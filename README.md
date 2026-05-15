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

## Auth & storage

Sign-in is via Firebase Authentication — Google popup or passwordless email link. The browser caches the session, so users stay signed in until they hit "Sign Out".

Player profiles and the global leaderboard share a single Firestore collection (project `fun-tools-mg`, collection `leaderboard`, doc id = Firebase Auth UID). The most recent leaderboard fetch is cached in `localStorage` under `mq:leaderboard` so the Hall of Fame still renders when offline.
