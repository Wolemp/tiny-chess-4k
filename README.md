# tiny-chess

A chess engine in under 4 KB of Python (make.fun tiny-chess-01).
`main.py` plays the gauntlet over HTTP; the engine itself is an lzma+base85 payload
unpacked at start-up: a 10x12 mailbox board kept from the mover's side, alpha-beta
with a transposition table, killer moves, null-move and late-move reductions,
quiescence search, a fixed node budget per move (no clock) and an endgame king
mop-up term. MIT.
