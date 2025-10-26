# Tic-TAC-TOE AI (C++)

A terminal-based Tic Tac Toe game featuring an unbeatable AI using the **Minimax algorithm with Alpha–Beta Pruning**.

## Features
- Human vs AI gameplay
- Optimal AI decisions
- Early win and delayed loss heuristics
- Clear and simple terminal interface

## How to Run
```bash
g++ src/tic_tac_toe.cpp -o tic_tac_toe
./tic_tac_toe
```
## Mini Max Algo with Alpha Beta Pruning:

The AI uses the Minimax algorithm, a decision-making method used in games like Tic Tac Toe,Othello,Chess.
It assumes both players play perfectly — the AI tries to maximize its chances of winning, while the opponent tries to minimize them-here is the catch "So AI in advance simulates the players minimizing move to predict in advance the best moves AI has and the paths it can avoid!".

Minimax looks at all possible future moves, simulates the game, and assigns scores:

+2000 for a win

0 for a draw

-2000 for a loss

The AI picks the move that leads to the best guaranteed outcome, assuming the opponent also plays optimally.

Alpha-Beta Pruning is an optimization that skips unnecessary paths:
if one move is already clearly better, it stops checking worse ones — this makes the AI much faster without changing the result.



Terminal UI:

X | - | -
----------
- | O | -
----------
- | - | X
