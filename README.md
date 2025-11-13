# ♟️ JavaScript Chess Game

A fully functional, browser-based chess game built completely with **vanilla JavaScript, HTML, and CSS**. The project plays like a lightweight chess engine inside the browser, with all major rules implemented accurately and a smooth, modern UI.

## 🚀 Features

### ✔ Full Chess Logic
- Accurate movement for all pieces
- Check, checkmate & stalemate detection
- Castling (King-side & Queen-side)
- En-passant capture
- Pawn promotion (Q, R, B, N) with user choice
- Turn-based play

### ✔ Smart Move Validation
- Generates pseudo-legal moves
- Filters out moves that expose the king
- Validates castling safety squares
- Tracks & restores:
  - En-passant rights
  - Castle rights
  - Promotions

### ✔ Move History + Notation
- Shows moves in clean **algebraic-style notation**
- Tracks moves turn-by-turn (1., 2., 3.…)
- Updates automatically on undo/redo and promotion

### ✔ Undo & Redo
- Fully reversible moves
- Restores board state, captures, promotions, castle rights, and en-passant status
- Redo stack clears on new moves

### ✔ UI & Experience
- Smooth board rendering
- Highlights selected piece, legal squares, and king-in-check
- Captured pieces display (for both sides)
- Flip board anytime (180° rotate)
- Animated result popup for wins/draws
- Clean piece images for all pieces

### ✔ Sound Effects
- Move
- Capture
- Check
- Castling
- Promotion
- Game ending

### ✔ Debug Helpers (for dev use)
```
window._chess.getBoard()
window._chess.doMove(...)
window._chess.undoMoveRecord(...)
window._chess.legalMovesFor(...)
window._chess.isKingInCheck(...)
```

## 🛠 Tech Stack
- **JavaScript (Vanilla)**
- **HTML**
- **CSS**
- Audio + PNG pieces for UI polish

## 📂 Project Structure
```
/audio        → move, capture, check, promote, castle, game-end sounds
/images       → all chess piece PNGs
script.js     → main game logic + rendering + engine
style.css     → board styles, highlights, UI
index.html    → page layout & containers
```

## 🎮 How to Play
1. Open `index.html` in any modern browser
2. Click a piece to highlight legal moves
3. Move pieces by selecting a target square
4. Undo/Redo moves anytime
5. Flip the board if you prefer the other angle
6. Play until checkmate, stalemate, or restart

## 🧩 Future Improvements
- PGN export
- AI opponent / engine integration
- Move hints or training mode
- Themes for board & pieces

## 💬 About the Project
I built this mainly to challenge myself to create a complete chess system from scratch using just vanilla JS, no frameworks, and no external engines. The logic, UI, state tracking, and game flow are all handcrafted and kept clean so it’s easy to modify or expand later.
