# ❌⭕ Tic-Tac-Toe with Minimax AI

A robust, command-line interface (CLI) Tic-Tac-Toe game built in Python. This project features a classic 2-player mode and an unbeatable single-player mode powered by the **Minimax algorithm**.

## 📋 Table of Contents
- [Features](#-features)
- [How to Play](#-how-to-play)
- [Installation & Usage](#-installation--usage)
- [Under the Hood: The AI](#-under-the-hood-the-ai)
- [Future Improvements](#-future-improvements)

## ✨ Features

* **Single Player Mode:** Challenge an AI that calculates the optimal move every turn.
* **Multiplayer Mode:** Play locally against a friend on the same computer.
* **Clean CLI:** Simple text-based interface for easy interaction.
* **Input Validation:** Prevents overwriting moves or entering invalid positions.

## 🎮 How to Play

The game is played on a 3x3 grid. The cells are numbered **1 through 9**, starting from the top-left corner.

**Board Key:**
```text
 1 | 2 | 3
---|---|---
 4 | 5 | 6
---|---|---
 7 | 8 | 9
```
When prompted, enter the number corresponding to the position where you want to place your mark (X or O).

Game Modes
Singleplayer: You play as X (goes first) vs. the Computer O.

Multiplayer: Player O goes first vs. Player X.

🚀 Installation & Usage
Prerequisites: You need to have Python installed on your machine.

1. Clone the repository:
```
git clone https://github.com/Yashika-28/tictactoe-minimax.git
```
2. Navigate to the project directory:
```
cd tictactoe-minimax
```
4. Run the script:
```
python main.py
```
🧠 Under the Hood: The AI
The single-player mode uses the Minimax Algorithm. This is a recursive backtracking algorithm used in decision theory and game theory.

How it works:
Look-ahead: The computer simulates all possible moves from the current state of the board.

Scoring: It assigns a score to terminal states:

+10 (AI wins)

-10 (Human wins)

0 (Draw)

Minimizing & Maximizing:

The AI (Maximizer) tries to get the highest score possible.

The AI assumes the Human (Minimizer) will play perfectly to get the lowest score possible.

Decision: It chooses the move that leads to the best possible outcome, assuming the opponent plays optimally. This makes the AI impossible to beat—the best result a human can achieve is a draw.

🔮 Future Improvements
[ ] Add a Graphical User Interface (GUI) using Tkinter or Pygame.

[ ] Add difficulty levels (Easy/Medium) by limiting the Minimax search depth or introducing random errors.

[ ] Refactor code into an Object-Oriented structure.
