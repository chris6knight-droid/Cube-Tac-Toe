# Cube Tac Toe

A browser game that fuses a 3×3 Rubik's Cube with Tic Tac Toe. Built with [Three.js](https://threejs.org/) in a single `index.html`.

## How to play

1. The cube has a black body with the classic Rubik's color scheme (white / yellow / red / orange / green / blue) so you can tell which way it's facing. **Drag empty space** to orbit and inspect every side; scroll/pinch to zoom. On phones it works in portrait — the cube auto-fits the screen.
2. On your turn:
   - **Place your mark** — tap any empty sticker (Player 1 = X, Player 2 = O). Marks have a white outline so they stay readable on every face color.
   - **Make one move** — click one of the 18 move buttons: faces `U U' D D' L L' R R' F F' B B'` or slices `M M' E E' S S'`. Your mark travels with its sticker.
3. **Win** by getting 3 of your marks in a row — horizontally, vertically, or diagonally — on a single 3×3 face. The win is checked **only after the rotation finishes**, never the instant you place a mark.

## Running it

ES-module imports don't load over `file://`, so serve the folder with any static server:

```bash
python3 -m http.server 8000
```

Then open <http://localhost:8000>.

Or just **double-click `Cube-Tac-Toe.html`** — a single self-contained file (Three.js inlined) that runs offline with no server.
