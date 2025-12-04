# Axelrod's Prisoner's Dilemma Tournament

A comprehensive web-based simulation of Robert Axelrod's famous Prisoner's Dilemma tournament, exploring the evolution of cooperation through game theory.

## 📚 Research Foundation

This project is based on Robert Axelrod's influential research paper, **"Effective Choice in the Prisoner's Dilemma"**, which made significant contributions to the fields of game theory, political science, and evolutionary biology.

Axelrod's work demonstrated how cooperation can emerge in a competitive environment of self-interested agents without a central authority. His tournament invited experts to submit computer programs (strategies) to play the Iterated Prisoner's Dilemma against each other. The surprising winner was the simplest strategy: **Tit for Tat**.

## 🎮 Simulation Features

This application brings Axelrod's tournament to life in your browser:

-   **15 Unique Strategies**: Includes classic strategies like *Tit for Tat*, *Friedman (Grudger)*, *Joss*, *Downing*, and more.
-   **Interactive Tournament Grid**: A 15x15 grid visualizing every match-up between strategies.
-   **Real-time Analysis**:
    -   **Match Details**: Click any cell to see a round-by-round timeline of moves (Cooperate vs. Defect).
    -   **Live Leaderboard**: Watch strategies climb or fall in rank as the tournament progresses.
    -   **Strategy Logic**: Click on any strategy name to learn how it makes decisions.
-   **Playback Controls**:
    -   **Auto-Play**: Watch the full 200-round tournament unfold automatically.
    -   **Step-by-Step**: Analyze the game one round at a time.
    -   **Speed Control**: (Internal variable) Adjustable simulation speed.

## 🧠 The Strategies

The simulation includes approximations of the following strategies:

1.  **Tit For Tat**: Cooperates on the first move, then copies the opponent's last move.
2.  **Tideman & Chieruzzi**: A complex strategy that retaliates but tries to break defect cycles.
3.  **Nydegger**: Uses a weighted formula of the last 3 outcomes.
4.  **Grofman**: Cooperates if moves match; otherwise, cooperates with a probability of 2/7.
5.  **Shubik**: Retaliates with increasing severity based on the number of times betrayed.
6.  **Stein & Rapoport**: Tit for Tat modification; cooperates first 4, defects last 2.
7.  **Friedman (Grudger)**: Cooperates until betrayed once, then defects forever.
8.  **Davis**: Cooperates for 10 rounds, then becomes a Grudger if betrayed.
9.  **Graaskamp**: Tit for Tat variant that defects on round 51 and periodically checks for weakness.
10. **Downing**: Estimates opponent's response probabilities to maximize expected yield.
11. **Feld**: Tit for Tat with a linearly decreasing probability of cooperation.
12. **Joss**: Tit for Tat but defects 10% of the time to try and exploit others.
13. **Tullock**: Cooperates based on the opponent's cooperation rate minus 10%.
14. **Name Withheld**: Tries to align behavior if the opponent is cooperative (>70%).
15. **Random**: The control strategy; 50/50 chance to Cooperate or Defect.

## 🚀 Getting Started

1.  Clone the repository.
2.  Open `index.html` in any modern web browser.
3.  Click **Auto-Play** to start the tournament or use **Step +1** to move manually.

## 🛠 Technologies Used

-   **HTML5**
-   **JavaScript (ES6+)**
-   **Tailwind CSS** (via CDN) for styling
-   **Chart.js** (via CDN)

## ⚠️ Disclaimer

The strategies implemented here are approximations based on descriptions from Robert Axelrod's *"The Evolution of Cooperation"*. As the original 1980 source code is not publicly available, specific implementation details (like exact random seeds, tie-breaking logic, or complex look-back depths) may differ slightly from the original tournament.
