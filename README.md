# tiny-chess-01

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/paimansilaen/tiny-chess-01/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/paimansilaen/tiny-chess-01/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A chess engine in a single `main.py` (Python 3.13, standard library only) for the make.fun tiny-chess-01 bounty. 0x88 board, alpha-beta search with iterative deepening to a fixed node budget (100,000 nodes a move), null-move pruning, transposition table with incremental Zobrist keys, MVV-LVA capture ordering, killer moves and a history heuristic, quiescence over captures, promotions and replies to a check. Evaluation is material plus piece-square tables, a bishop-pair bonus and a separate king table for queenless endgames. Deterministic: no clock, no unseeded randomness, no model calls. `main.py` holds the engine as a compressed (zlib + base85) payload, which counts toward the 4,096-byte cap.

## Run it

```sh
MAKEFUN_ENV_URL=http://localhost:8080 python3 main.py
```

---

<sub>Entered on [make.fun](https://make.fun/?ref=4gn3z50j&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
