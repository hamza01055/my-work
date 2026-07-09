# 🎮 Tic-Tac-Toe vs AI (Minimax Algorithm)

Day 4 of improving my skills — a Tic-Tac-Toe game where you play against an **unbeatable AI opponent** built with the **minimax algorithm** and **alpha-beta pruning**.

No libraries, no frameworks — just one HTML file with plain JavaScript.

## 🚀 How to run

Just open `index.html` in any browser. That's it.

Or play it online by enabling **GitHub Pages** in this repo's settings (Settings → Pages → deploy from `main` branch).

## 🧠 How the AI works

Before every move, the AI simulates **every possible future game** from the current position:

1. It tries a move, then imagines your best possible reply, then its best reply to that, and so on until the game ends.
2. Each end state gets a score: **+10** if the AI wins, **-10** if you win, **0** for a draw (adjusted by depth so it wins fast and loses slow).
3. It assumes you also play perfectly (that's the "minimax" part — it **maximizes** its score while you **minimize** it).
4. **Alpha-beta pruning** lets it skip branches that can't change the outcome, making the search much faster.

The result: the AI never loses. The best you can achieve is a draw. The footer shows how many game states it explored for each move.

## 📚 What I learned

- Recursion and game-tree search
- The minimax algorithm and alpha-beta pruning
- DOM manipulation and event handling in vanilla JS
- CSS Grid, custom properties, and accessibility basics (focus states, reduced motion)

## 🔮 Ideas to extend

- Difficulty levels (make the AI sometimes pick a random move)
- Connect Four with the same algorithm + depth limit
- Show the AI's score for each candidate move on hover
