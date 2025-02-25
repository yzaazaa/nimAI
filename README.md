# Nim AI

**Introduction**

This Python implementation provides a reinforcement learning model that plays the game of **Nim** using **Q-learning**. The algorithm learns optimal strategies by playing against itself and improving over time. Key features include:

* **Game Implementation:**
  * Simulates the game of Nim with configurable initial conditions.
  * Allows for both human and AI players.

* **Reinforcement Learning with Q-Learning:**
  * Uses Q-learning to estimate the best moves.
  * Updates Q-values based on rewards from past experiences.

* **Training AI:**
  * Self-plays multiple games to improve its strategy.
  * Stores learned Q-values for future decision-making.

* **AI vs Human Play:**
  * Enables playing against the trained AI model.
  * AI selects moves based on learned Q-values.

**Usage**
1. Clone the Repository:
```bash
git clone https://github.com/yzaazaa/nimAI
cd nimAI
```

2. Run the script:
```bash
python play.py
```

**API Reference**

The script provides functions for training and playing the Nim game.

* **train(n):**

* Trains the AI by playing n games against itself.
* Returns a dictionary of Q-values.

* **play(q_values):**

* Allows a human to play against the trained AI.
* Uses learned Q-values to make decisions.

* **best_move(state, q_values):**

* Determines the best move given a state and learned Q-values.

* **update_q_value(q_values, state, action, new_state, reward, alpha, gamma):**

* Updates Q-values based on reinforcement learning principles.