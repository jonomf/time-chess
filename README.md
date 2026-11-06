# TIME CHESS!

Chess in the browser with visual overlays and branching timelines.

- **Square control map**: every square shaded by who attacks it (counted from White's side), with outnumbered pieces flagged and move safety shown as you pick a piece. Tap an empty square to see which pieces attack it, or any piece to see what protects and attacks it.
- **Play Stockfish or a friend**: Stockfish plays Black by default, with a 1–10 difficulty slider.
- **Branching timelines**: go back to any move and play something else; the old line stays. Simulate any position forward with Stockfish. An interactive branch tree shows every line; tap any move in it to jump there.
- **Timeline ribbon**: one card per move under the board, with the engine's evaluation graph drawn at the same scale and blunders, mistakes and strong moves marked.
- **Coach mode**: Coach Pip names your opening and offers book moves, gives a nudge or the engine's best move with a plain-language reason, grades your last move, and flags pieces in danger. Switch it to **Rate my moves** to play with no hints: each move gets rated afterward, with the engine's better options and a button to replay one as a new branch.
- **Creative mode**: drag any piece anywhere, drop it off the board to remove it, or place pieces from a palette, and set who moves next. Legal moves still count as moves; everything else is recorded as an edit in the timeline, so you can rewind it. Stockfish keeps evaluating, and you can play on from your setup.
- **Story Mode**: trace any piece's path through the game, see the standout pieces and their stories, and jump to the biggest turning points to branch from them.

- **Go mode**: switch to Go from the header and get the same tools for Go: 9×9, 13×13 or 19×19 boards, a Monte Carlo computer opponent, a territory map, atari warnings, win-chance timeline, branch tree, coach, story mode and simulation.
- **Online play**: host a chess or Go game from the Online tab and send a friend the 6-character code or invite link. Browsers connect directly over WebRTC; PeerJS's public server is used only to introduce them.
- **Solitaire and Sudoku**: two one-player modes with the same tools: a timeline with a progress graph, a branch tree for rewinding and trying other lines, coach hints, Story Mode, simulation and both skins. Solitaire is Klondike (draw 1 or 3) with tap-to-move and drag, and every deal is checked by a built-in solver before it's dealt, so it can always be won; Sudoku generates unique-solution puzzles at three levels, with notes, a candidate map, mistake checking, and coach overlays that show where a number can go, what rules numbers out of a square, which squares are solvable now, and a heat map of remaining options.

It's a single `index.html` with no build step. Chess rules come from [chess.js](https://github.com/jhlywa/chess.js) and the engine is [Stockfish.js](https://github.com/nmrugg/stockfish.js), both loaded from cdnjs. The Go engine is a small Monte Carlo search built into the page.
