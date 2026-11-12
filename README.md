# Tiny Chess — 4 KB Python chess engine

A 4,096-byte Python chess engine for the make.fun tiny-chess-01 competition, entry for @gm-xbt.

Alpha-beta search with quiescence, transposition table, and killer move ordering.
Fixed budget of 50,000 nodes per move — fully deterministic, stdlib only.

Round 2 fixed an en-passant Zobrist hash bug that flipped a trial game.
Packed trial-0 Elo: 1,326 (3W/1D/4L) on the house scorer, above the 1,154 final floor.

Run it locally: `python3 main.py` reads a position from stdin and prints the best move.
