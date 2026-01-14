# Algorithmic Poker Bot

A quantitative poker agent designed for competitive algorithmic trading simulations. This bot uses Monte Carlo simulations to calculate hand equity in real-time and adjusts its strategy based on opponent behavior modeling.

## Key Features

* **Monte Carlo Simulation:** Runs thousands of random scenarios per hand to calculate the exact probability of winning (Equity) against unknown opponent cards.
* **Dynamic Opponent Modeling:**
    * **"Bully" Detection:** Identifies opponents who bluff frequently and loosens calling thresholds.
    * **"Calling Station" Logic:** Tightens ranges against players who rarely fold.
* **Expected Value (EV) Engine:** Makes decisions (Fold/Call/Raise) based on pot odds and statistical positive expectation.
* **End-Game Optimization:** Adjusts risk appetite based on the current score differential to protect leads or chase deficits.

## Tech Stack
* **Language:** Python 3
* **Concepts:** Game Theory, Probability Statistics, Monte Carlo Methods

## How to Run

1. Ensure you have Python installed.
2. Run the script:
   ```bash
   python3 poker_bot.py

## Note: The bot expects JSON state input via STDIN as per standard competition protocols.
