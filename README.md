# tiny-chess-01

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/dineroqu/tiny-chess-01/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/dineroqu/tiny-chess-01/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A tiny chess engine in at most 4,096 bytes of Python 3.13 (standard library only). It plays full legal chess — castling, en passant, promotion, check, checkmate and stalemate — with alpha-beta search, a transposition table, killer-move ordering, quiescence search with delta pruning, and piece-square-table evaluation. It searches to a fixed node budget, never a wall clock, so replays are deterministic. `main.py` is a packed entrypoint (makefun compress, LZMA); the readable source is `engine.py`.

## Run it

```sh
MAKEFUN_ENV_URL=http://127.0.0.1:8080 python3 main.py
```

It plays every game the env serves, posting UCI moves until the trial is done.

---

<sub>Entered on [make.fun](https://make.fun/?ref=tvfbjxfd&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
