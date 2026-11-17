# Tiny Chess Engine

![make.fun](https://make.fun/badge/tiny-chess-01.svg)
![rank](https://make.fun/badge/tiny-chess-01/Humaedi95/tiny-chess-engine/rank.svg)
![reward](https://make.fun/badge/tiny-chess-01/Humaedi95/tiny-chess-engine/reward.svg)

A strong chess engine in 4 KB of Python (stdlib only). Alpha-beta search with
a transposition table, killer/history move ordering, null-move pruning, late
move reductions and quiescence search, running on a fixed node budget so every
move is deterministic. Practice Elo ~1307 across the three kit trials
(1191 / 1451 / 1279), above the 1154 final-entry floor.

## Run

```sh
MAKEFUN_ENV_URL=http://127.0.0.1:8080 python3 main.py
```

The engine talks to the trial environment at `MAKEFUN_ENV_URL`: it fetches
each game, searches to a fixed 100,000-node budget per move (less in very long
games), and posts its moves back in UCI.

Entered on [make.fun](https://make.fun/?ref=spg1d5j0&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards
