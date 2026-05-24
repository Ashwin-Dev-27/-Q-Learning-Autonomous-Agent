<div align="center">

# ✨ Q Learning Autonomous Agent ✨

[![Status](https://img.shields.io/badge/Status-Active-success.svg)]()
[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)]()
[![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)]()
[![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)]()


</div>

---

# 🤖 Q-Learning Pathfinding Agent

### An implementation of Reinforcement Learning to solve navigation problems.

This project demonstrates the core concepts of **Reinforcement Learning (RL)** by training an autonomous agent to navigate a 2D grid environment (Maze/Chip Design) to reach a goal while avoiding obstacles. It uses the **Q-Learning algorithm** to learn the optimal policy through trial and error.

---

## 🧠 What is this?

Unlike traditional programming where we tell the computer exactly *how* to move, in Reinforcement Learning, we tell the computer *what is good* (Reward) and *what is bad* (Penalty). The agent figures out the "how" on its own.

**Key Concepts Implemented:**
* **Q-Table:** A lookup table where the agent stores the "value" of taking a specific action in a specific state.
* **Exploration vs. Exploitation:** Balancing trying new paths (randomness) vs. sticking to what works (using the Q-Table).
* **Bellman Equation:** The math used to update the Q-values based on future rewards.

---

## 🛠️ Tech Stack

* **Language:** Python 3.x
* **Libraries:** NumPy (for Matrix operations), Matplotlib (for visualization)
* **Algorithm:** Q-Learning (Off-policy TD control)

---

## ⚙️ How It Works

1.  **Environment Setup:** A grid is initialized with a **Start Point**, a **Goal**, and **Obstacles** (Walls/Holes).
2.  **Training Loop:**
    * The Agent starts at a random position.
    * It chooses an action (Up, Down, Left, Right).
    * **Reward System:**
        * Hit Obstacle: **-10 Points** (Punishment)
        * Open Step: **-1 Point** (Small punishment to encourage speed)
        * Reach Goal: **+100 Points** (Reward)
    * The Q-Table is updated.
3.  **Result:** After thousands of episodes, the agent "learns" the shortest path without ever being explicitly programmed with the route.

---

## 🚀 How to Run

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/Ashwin-Dev-27/RL-Pathfinder.git](https://github.com/Ashwin-Dev-27/RL-Pathfinder.git)
    ```
2.  **Run the training script:**
    ```bash
    python train_agent.py
    ```
3.  **Watch the output:** You will see the "Success Rate" increase as the agent gets smarter over time.

---

### 📝 Author
**Ashwin Kumar**
*B.Tech Computer Science*
