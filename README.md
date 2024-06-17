# Reinforcement-learning-RL-Project-1
Bandit Learning Algorithms

# Multi-Armed Bandit Algorithm

## Overview
This project aims to experiment with simple bandit learning algorithms by implementing them from scratch. The performance of these algorithms will be compared based on two criteria:

  **1.** Average Accumulated Reward: The total reward accumulated over time.
  
  **2.** Proportion of Optimal Action: The frequency of selecting the action with the highest expected reward.

## Requirements
**Python Version:** 3.9.12

## Libraries
**numpy:** 1.26.2

**matplotlib:** 3.8.3

## Functions
The primary function in this project is **MultiArmedBandit**, which is capable of executing all required methods. The parameters can be adjusted to use a specific method. Here are the details of the parameters:

*  **'n'** (default=10): Number of arms.
* **'steps'** (default=1000): Number of attempts for exploration and exploitation.
* **'method'** (default='greedy'): Method to be used. Options are ['greedy', 'epsilon', 'optimistic', 'gradient'].
* **'Alpha'** (default=0.1): Alpha value for the gradient method.
* **'NonStationary'** (default='drift'): Non-stationary rewards. Options are ['drift', 'reverting'].
* **'Permute_Prob'** (default=0): Probability of an abrupt change at each step.
* **'Step'** (default=None): Step size for epsilon-fixed size. If **None**, a decreasing step size is used.

  
