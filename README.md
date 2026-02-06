# 🧩 Sudoku Fun!

A colorful, kid-friendly 9×9 Sudoku game built with plain HTML, CSS, and JavaScript. No frameworks, no dependencies — just open and play!

**[▶️ Play Now](https://alfredang.github.io/sudoku/)**

![Menu Screen](screenshots/menu.png)
![Game Screen](screenshots/game.png)

## ✨ Features

- **3 Difficulty Levels** — Easy (15 min), Medium (10 min), Hard (5 min)
- **Countdown Timer** — Pulses red when under 30 seconds
- **Click-to-Play** — Tap cells and number buttons (no keyboard needed)
- **Rule Validation** — Highlights conflicts in red with friendly messages
- **Win Detection** — Celebration animation when you solve the puzzle
- **Give Up** — Reveals the full solution with color-coded answers
- **Solution Reveal Colors:**
  - ⬛ **Black** — Original given numbers
  - 🔵 **Blue** — Your correct entries
  - 🟢 **Green** — Auto-revealed answers
- **Responsive Design** — Works on desktop, tablet, and mobile

## 🚀 Getting Started

### Play Online

Visit **[alfredang.github.io/sudoku](https://alfredang.github.io/sudoku/)**

### Run Locally

```bash
git clone https://github.com/alfredang/sudoku.git
cd sudoku
open index.html
```

No build step, no install — just open the HTML file in any browser.

## 📁 Project Structure

```
sudoku/
├── index.html          # Main HTML page
├── css/
│   └── style.css       # All styles (colors, grid, responsive)
├── js/
│   └── game.js         # Game logic (generation, validation, timer)
├── screenshots/        # README screenshots
├── .github/
│   └── workflows/
│       └── deploy.yml  # GitHub Pages auto-deploy
└── README.md
```

## 🧠 How It Works

1. **Puzzle Generation** — A backtracking algorithm fills a valid 9×9 grid, then randomly removes cells based on difficulty
2. **Validation** — Each entry is checked against Sudoku rules (row, column, and 3×3 box) — not just the answer key — so players learn *why* a number doesn't fit
3. **Solution Verification** — Every generated board is validated to ensure all rows, columns, and boxes contain digits 1–9 (each summing to 45)

## 🛠️ Tech Stack

- HTML5
- CSS3 (Grid, Custom Properties, Animations)
- Vanilla JavaScript (ES6+)
- GitHub Actions for deployment

## 📄 License

MIT
