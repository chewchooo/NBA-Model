# NBA-Model

Hosted data and page for **NBA Edge**, a player projection board for an NBA slate.

- `nba-edge/index.html` — the board, self-contained apart from the data beside it
- `nba-edge/data.js` — the current slate
- `nba-edge/meta.js` — a small stamp the page polls, so a shared copy fetches the
  full data file only when it has actually changed

**This repository is a delivery mechanism, not the project.** The model, the backtest
and every measurement live in the Jarvis vault; only built artefacts are published here.
The history is deliberately held at a single commit — a 1 MB data file recommitted daily
would grow the repo by that much each time for nothing.

## What the board does and does not claim

It ranks SPOTS: how much better than his own average a player's night projects to be.
There is **no odds feed for player props**, so it is not an edge against a price. Every
market carries an honest verdict, including the ones that do not beat doing nothing.

The game-outcome model **loses to the closing spread** (MAE 10.10 against 9.81 on 606
games of 2022-23), and says so.
