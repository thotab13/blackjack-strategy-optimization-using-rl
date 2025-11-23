# Blackjack Reinforcement Learning Project 🃏

This project implements and compares multiple strategies for playing Blackjack using **Reinforcement Learning (RL)**.  
Starting from a simple fixed strategy, it evolves into a **self-learning agent** with **card counting** and **adaptive betting** designed to maximize long-term profit.

The core goal is to demonstrate how RL agents (using **Q-Learning** and **SARSA**) can learn an **optimal policy** in the stochastic environment of Blackjack.

---

## 🎯 Objectives

- Build a flexible Blackjack simulation environment with configurable rules.
- Implement **baseline strategies** (e.g., Thorp’s Basic Strategy) for comparison.
- Train **Q-Learning** and **SARSA** agents to learn optimal play from experience.
- Extend the agent with a **Hi-Lo card counting system** and **adaptive betting strategy**.
- Visualize learning performance and policy behavior over time.

---

## ✨ Features

This project implements code and logic for:

### 🃠 Flexible Blackjack Environment
- Custom-built environment for simulating Blackjack.
- Supports:
  - Configurable **number of decks**.
  - Common **casino rule variations** such as:
    - **H17** – Dealer hits on soft 17.
    - **No Double Down** – Player cannot double their bet.
- Designed to be extensible for additional rule variations.

### 📘 Thorp’s Basic Strategy (Baseline)
- Functional implementation of **Edward O. Thorp’s Basic Strategy**.
- Serves as a **non-learning baseline** for benchmarking RL agents.
- Useful for comparing how much RL improves over a strong human-derived strategy.

### 🤖 Q-Learning Agent (Off-Policy RL)
- Implementation of **Q-Learning** for Blackjack.
- Learns an approximate optimal policy purely from simulated experience.
- Uses an **off-policy** update rule, allowing exploration policies different from the greedy policy.

### 🧠 SARSA Agent (On-Policy RL)
- Implementation of the **SARSA** algorithm.
- Provides a direct **on-policy** counterpart to Q-Learning.
- Useful for analyzing differences in learning dynamics between SARSA and Q-Learning.

### 🔢 Point-Count System (Hi-Lo)
- Advanced agent includes a **dual-parameter Hi-Lo card counting system**.
- Tracks the changing value of the remaining deck(s).
- Uses the count to drive an **adaptive betting strategy** aimed at maximizing profit over many hands.
