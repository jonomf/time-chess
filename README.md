# TIME CHESS!

Chess in the browser with visual overlays and branching timelines.

- **Square control map**: every square shaded by who attacks it (counted from White's side), with outnumbered pieces flagged and move safety shown as you pick a piece. Tap an empty square to see which pieces attack it, or any piece to see what protects and attacks it.
- **Play Stockfish or a friend**: Stockfish plays Black by default, with a 1–10 difficulty slider.
- **Branching timelines**: go back to any move and play something else; the old line stays. Simulate any position forward with Stockfish. An interactive branch tree shows every line; tap any move in it to jump there.
- **Timeline ribbon**: one card per move under the board, with the engine's evaluation graph drawn at the same scale and blunders, mistakes and strong moves marked.
- **Coach mode**: Coach Pip names your opening and offers book moves, gives a nudge or the engine's best move with a plain-language reason, grades your last move, and flags pieces in danger.
- **Story Mode**: trace any piece's path through the game, see the standout pieces and their stories, and jump to the biggest turning points to branch from them.

- **Go mode**: switch to Go from the header and get the same tools for Go: 9×9, 13×13 or 19×19 boards, a Monte Carlo computer opponent, a territory map, atari warnings, win-chance timeline, branch tree, coach, story mode and simulation.
- **Online play**: host a chess or Go game from the Online tab and send a friend the 6-character code or invite link. Browsers connect directly over WebRTC; PeerJS's public server is used only to introduce them.

It's a single `index.html` with no build step. Chess rules come from [chess.js](https://github.com/jhlywa/chess.js) and the engine is [Stockfish.js](https://github.com/nmrugg/stockfish.js), both loaded from cdnjs. The Go engine is a small Monte Carlo search built into the page.
