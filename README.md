# Customizing OpenAI Gym Environments and Implementing Reinforcement Learning Agents
# Overview
This project customizes the Taxi-v3 environment from OpenAI Gym and implements reinforcement learning (RL) agents using Stable-Baselines3. The main focus is to enhance the environment by introducing new actions and reward mechanisms, and evaluate their effects on the performance of three RL algorithms: PPO (Proximal Policy Optimization), A2C (Advantage Actor-Critic), and DQN (Deep Q-Network).

# Features
Environment
Base Environment: Taxi-v3, a 5x5 grid-based environment where the taxi must pick up and drop off passengers at designated locations.
# Customizations:
Action Wrapper: Adds diagonal movements to the action space.
Reward Wrapper: Penalizes revisiting recently visited locations to discourage inefficient exploration.
# RL Algorithms
PPO (Proximal Policy Optimization): Balances exploration and exploitation with stable updates.
A2C (Advantage Actor-Critic): Combines policy-based and value-based methods for efficient learning.
DQN (Deep Q-Network): Utilizes deep learning for value approximation in discrete action spaces.
# Hyperparameter Tuning
Conducted using multiprocessing to identify the optimal configurations for each algorithm.
# Results
The performance of the baseline and customized environments was evaluated for each RL algorithm.
Results were compared using metrics like average rewards and training stability.
Customizations showed varying impacts on performance:
Action customization improved navigation efficiency.
Reward customization discouraged redundant movements.
Combined customizations provided the best overall improvement.
