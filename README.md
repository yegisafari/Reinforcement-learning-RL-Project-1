# Reinforcement-Learning-RL-Project-1
Bandit Learning Algorithms

# Multi-Armed Bandit Algorithm

## Overview
This project is all about experimenting with simple bandit learning algorithms by building them from scratch. We'll be comparing how well these algorithms perform based on two main criteria:

  **1.** **Average Accumulated Reward:** The total reward accumulated over time.
  
  **2.** **Proportion of Optimal Action:** The frequency of selecting the action with the highest expected reward.

## Requirements
**Python Version:** 3.9.12

## Libraries
**numpy:** 1.26.2

**matplotlib:** 3.8.3

## Functions
The key function here is **MultiArmedBandit**, which handles all the methods we need. You can tweak the parameters to choose a specific method. Here's a quick rundown of the parameters:

*  **'n'** (default=10): Number of arms.
* **'steps'** (default=1000): Number of attempts for exploration and exploitation.
* **'method'** (default='greedy'): Method to be used. Options are ['greedy', 'epsilon', 'optimistic', 'gradient'].
* **'Alpha'** (default=0.1): Alpha value for the gradient method.
* **'NonStationary'** (default='drift'): Non-stationary rewards. Options are ['drift', 'reverting'].
* **'Permute_Prob'** (default=0): Probability of an abrupt change at each step.
* **'Step'** (default=None): Step size for epsilon-fixed size. If **None**, a decreasing step size is used.

## Execution Instructions

We've designed this project to be run in Google Colab. The code is divided into different sections, each in its own cell. 
To get started:

**1.** Open Google Colab and upload the notebook.

**2.** Run each cell one by one from top to bottom.

**3.** The whole process should take around 15 minutes.

## Steps to Run in Google Colab

**1.** **Open Google Colab:** Head over to [Google Colab](https://colab.research.google.com/).

**2.** **Upload Notebook:** Click on the "File" menu and select "Upload notebook." Choose the **.ipynb** file from your computer.

**3.** **Run Cells:** Click the "Run" button or press **Shift + Enter** to run each cell in the notebook.

## Usage Example
You can customize the **MultiArmedBandit function** according to your needs. Here’s an example:

``` 
from multi_armed_bandit import MultiArmedBandit

# Example 
result = MultiArmedBandit(n=10, steps=1000, method='epsilon', Alpha=0.1, NonStationary='drift', Permute_Prob=0.1, Step=0.01)
```

## Additional Notes

**Exploration vs Exploitation:** One of the key challenges in multi-armed bandit problems is finding the right balance between exploring new actions and exploiting actions that are known to be rewarding.

**Non-Stationary Environments:** In real-life scenarios, reward probabilities can change over time. This project includes non-stationary environments to make things more realistic and challenging.

**Evaluation Metrics:** To understand how effective our algorithms are, we'll focus on two main metrics: average accumulated reward and the proportion of times the optimal action is chosen.

Feel free to dive into the code and play around with the parameters to see how different strategies perform. If you have any questions or run into any issues, don't hesitate to open an issue in the repository.



