<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tic-Tac-Toe with Minimax AI - Project Documentation</title>
    <style>
        body {
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, Arial, sans-serif;
            line-height: 1.6;
            color: #24292e;
            max-width: 800px;
            margin: 0 auto;
            padding: 20px;
        }
        h1, h2, h3 {
            margin-top: 24px;
            margin-bottom: 16px;
            font-weight: 600;
            line-height: 1.25;
        }
        h1 {
            font-size: 2em;
            border-bottom: 1px solid #eaecef;
            padding-bottom: 0.3em;
        }
        h2 {
            font-size: 1.5em;
            border-bottom: 1px solid #eaecef;
            padding-bottom: 0.3em;
        }
        h3 {
            font-size: 1.25em;
        }
        code {
            padding: 0.2em 0.4em;
            margin: 0;
            font-size: 85%;
            background-color: #f6f8fa;
            border-radius: 3px;
            font-family: "SFMono-Regular", Consolas, "Liberation Mono", Menlo, Courier, monospace;
        }
        pre {
            padding: 16px;
            overflow: auto;
            font-size: 85%;
            line-height: 1.45;
            background-color: #f6f8fa;
            border-radius: 3px;
        }
        pre code {
            padding: 0;
            background-color: transparent;
        }
        blockquote {
            padding: 0 1em;
            color: #6a737d;
            border-left: 0.25em solid #dfe2e5;
            margin: 0;
        }
        ul {
            padding-left: 2em;
        }
        a {
            color: #0366d6;
            text-decoration: none;
        }
        a:hover {
            text-decoration: underline;
        }
        .board-key {
            font-family: monospace;
            white-space: pre;
            background: #f6f8fa;
            padding: 10px;
            border-radius: 5px;
            display: inline-block;
        }
    </style>
</head>
<body>

    <h1>❌⭕ Tic-Tac-Toe with Minimax AI</h1>

    <p>A robust, command-line interface (CLI) Tic-Tac-Toe game built in Python. This project features a classic 2-player mode and an unbeatable single-player mode powered by the <strong>Minimax algorithm</strong>.</p>

    <h2>📋 Table of Contents</h2>
    <ul>
        <li><a href="#features">Features</a></li>
        <li><a href="#how-to-play">How to Play</a></li>
        <li><a href="#installation">Installation & Usage</a></li>
        <li><a href="#ai">Under the Hood: The AI</a></li>
        <li><a href="#future">Future Improvements</a></li>
    </ul>

    <h2 id="features">✨ Features</h2>
    <ul>
        <li><strong>Single Player Mode:</strong> Challenge an AI that calculates the optimal move every turn.</li>
        <li><strong>Multiplayer Mode:</strong> Play locally against a friend on the same computer.</li>
        <li><strong>Clean CLI:</strong> Simple text-based interface for easy interaction.</li>
        <li><strong>Input Validation:</strong> Prevents overwriting moves or entering invalid positions.</li>
    </ul>

    <h2 id="how-to-play">🎮 How to Play</h2>
    <p>The game is played on a 3x3 grid. The cells are numbered <strong>1 through 9</strong>, starting from the top-left corner.</p>

    <h3>Board Key:</h3>
    <div class="board-key">
 1 | 2 | 3
---|---|---
 4 | 5 | 6
---|---|---
 7 | 8 | 9
    </div>

    <p>When prompted, enter the number corresponding to the position where you want to place your mark (X or O).</p>

    <h3>Game Modes</h3>
    <ol>
        <li><strong>Singleplayer:</strong> You play as <strong>X</strong> (goes first) vs. the Computer <strong>O</strong>.</li>
        <li><strong>Multiplayer:</strong> Player <strong>O</strong> goes first vs. Player <strong>X</strong>.</li>
    </ol>

    <h2 id="installation">🚀 Installation & Usage</h2>
    <p><strong>Prerequisites:</strong> You need to have <a href="https://www.python.org/downloads/">Python</a> installed on your machine.</p>

    <ol>
        <li>
            <strong>Clone the repository:</strong>
            <pre><code>git clone https://github.com/your-username/tictactoe-minimax.git</code></pre>
        </li>
        <li>
            <strong>Navigate to the project directory:</strong>
            <pre><code>cd tictactoe-minimax</code></pre>
        </li>
        <li>
            <strong>Run the script:</strong>
            <pre><code>python main.py</code></pre>
            <p><em>(Note: Replace <code>main.py</code> with the name of your python file)</em></p>
        </li>
    </ol>

    <h2 id="ai">🧠 Under the Hood: The AI</h2>
    <p>The single-player mode uses the <strong>Minimax Algorithm</strong>. This is a recursive backtracking algorithm used in decision theory and game theory.</p>

    <h3>How it works:</h3>
    <ol>
        <li><strong>Look-ahead:</strong> The computer simulates all possible moves from the current state of the board.</li>
        <li><strong>Scoring:</strong> It assigns a score to terminal states:
            <ul>
                <li><strong>+10</strong> (AI wins)</li>
                <li><strong>-10</strong> (Human wins)</li>
                <li><strong>0</strong> (Draw)</li>
            </ul>
        </li>
        <li><strong>Minimizing & Maximizing:</strong>
            <ul>
                <li>The AI (Maximizer) tries to get the highest score possible.</li>
                <li>The AI assumes the Human (Minimizer) will play perfectly to get the lowest score possible.</li>
            </ul>
        </li>
        <li><strong>Decision:</strong> It chooses the move that leads to the best possible outcome, assuming the opponent plays optimally. This makes the AI impossible to beat—the best result a human can achieve is a draw.</li>
    </ol>

    <h2 id="future">🔮 Future Improvements</h2>
    <ul class="task-list">
        <li><input type="checkbox" disabled> Add a Graphical User Interface (GUI) using Tkinter or Pygame.</li>
        <li><input type="checkbox" disabled> Add difficulty levels (Easy/Medium) by limiting the Minimax search depth.</li>
        <li><input type="checkbox" disabled> Refactor code into an Object-Oriented structure.</li>
    </ul>

    <h2>🤝 Contributing</h2>
    <p>Contributions, issues, and feature requests are welcome!</p>

    <h2>📄 License</h2>
    <p>This project is open source.</p>

</body>
</html>
