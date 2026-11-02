# TIME CHESS!

Chess in the browser with visual overlays and branching timelines.

- **Square control map**: every square shaded by who attacks it (counted from White's side), with outnumbered pieces flagged and move safety shown as you pick a piece.
- **Play Stockfish or a friend**: Stockfish plays Black by default, with a 1–10 difficulty slider.
- **Branching timelines**: go back to any move and play something else; the old line stays. Simulate any position forward with Stockfish.
- **Timeline ribbon**: one card per move under the board, with the engine's evaluation graph drawn at the same scale and blunders, mistakes and strong moves marked.
- **Review**: trace any piece's path through the game, see the standout pieces and their stories, and jump to the biggest turning points to branch from them.

It's a single `index.html` with no build step. Chess rules come from [chess.js](https://github.com/jhlywa/chess.js) and the engine is [Stockfish.js](https://github.com/nmrugg/stockfish.js), both loaded from cdnjs.
