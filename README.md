# ♟️ Advanced Chess Game with Python-Chess

> A feature-rich, GUI-based chess game built with **Pygame** and powered by the **python-chess** library for full game logic, AI, and move validation.

---

## 🎮 Preview

```
♜ ♞ ♝ ♛ ♚ ♝ ♞ ♜   ← Black pieces
♟ ♟ ♟ ♟ ♟ ♟ ♟ ♟
· · · · · · · ·
· · · · · · · ·
· · · · · · · ·
· · · · · · · ·
♙ ♙ ♙ ♙ ♙ ♙ ♙ ♙
♖ ♘ ♗ ♕ ♔ ♗ ♘ ♖   ← White pieces
```

---

## ✨ Features

- ✅ **Full Chess Rules** — Powered by `python-chess` for legal move validation, castling, en passant, promotion, and check/checkmate detection
- 🖼️ **Pygame GUI** — Clean visual board with Unicode chess piece rendering
- 🤖 **AI Bot** — Built-in AI opponent (`ai/ai_bot.py`) for single-player mode
- 🔊 **Sound Effects** — Move, capture, and castle sounds with toggle support
- 📜 **Move History** — Full game history viewer (press `H`)
- ⚖️ **Material Tracker** — Live material balance display
- 🔄 **Board Flip** — Flip the board to play from either side (press `F`)
- ♟️ **Captured Pieces** — Visual display of captured material

---

## 🗂️ Project Structure

```
Chess_game 2.0/
├── my_chess_game/
│   ├── ai/
│   │   └── ai_bot.py          # AI logic and move evaluation
│   ├── gui/
│   │   ├── pygame_gui.py      # Main GUI — board rendering, events, game loop
│   │   └── prototype.py       # Prototype/test GUI
│   ├── assets/                # Sound files and piece images (13 piece images)
│   └── main.py                # Entry point
└── README.md
```

---

## 🚀 Getting Started

### Prerequisites

```bash
Python 3.12+
pygame
python-chess
```

### Installation

```bash
# Clone the repository
git clone https://github.com/soala7/chess-python.git
cd chess-python

# Create and activate a virtual environment (recommended)
python -m venv venv
source venv/bin/activate        # Linux/macOS
venv\Scripts\activate           # Windows

# Install dependencies
pip install pygame python-chess
```

### Run the Game

```bash
python my_chess_game/main.py
```

---

## 🕹️ Controls

| Key / Action | Description |
|---|---|
| `Click` | Select and move a piece |
| `R` | Reset the game |
| `H` | Show full move history |
| `F` | Flip the board view |
| `S` | Toggle sound on/off |
| `ESC` | Quit the game |

---

## 🧠 How It Works

### Game Logic
All chess rules are handled by the `python-chess` library, including:
- Legal move generation
- Check, checkmate, and stalemate detection
- En passant and castling
- Pawn promotion

### Rendering
`PieceRenderer` loads 13 piece images from the assets folder and falls back to Unicode symbols if images are unavailable. The board updates in real time after every move.

### AI Bot
The AI (`ai_bot.py`) evaluates positions and returns the best move for the opponent. It integrates directly with the `python-chess` board state.

---

## 📦 Dependencies

| Package | Purpose |
|---|---|
| `pygame` | GUI rendering, events, and sound |
| `python-chess` | Chess rules, move validation, board state |

---

## 🛠️ Built With

- **Python 3.12**
- **Pygame** — 2D game library for rendering and input
- **python-chess** — Chess logic and move generation

---

## 🤝 Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you'd like to change.

1. Fork the repository
2. Create your feature branch: `git checkout -b feature/your-feature`
3. Commit your changes: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin feature/your-feature`
5. Open a Pull Request

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

## 👤 Author

**soala7**
- GitHub: [@soala7](https://github.com/soala7)
- Want to challange me? search soalasnk on Chess.com

---

> *"Every chess master was once a beginner."* — Irving Chernev
