# Reinforcement Learning Lab Work

This repository contains 10 practical programs implementing fundamental reinforcement learning algorithms and techniques, from basic bandit problems to policy gradient methods.

## Programs Overview

### Program 1: Epsilon-Greedy Multi-Armed Bandit for Ad Placement
- Implemented epsilon-greedy strategy for online ad optimization
- Simulated click-through rates (CTR) for different ad slots (0.05, 0.07, 0.02, 0.1)
- Balanced exploration (10%) vs exploitation (90%)
- Tracked cumulative clicks over 1000 impressions
- Results: Sidebar (62 clicks) performed best, demonstrating effective slot selection

**Screenshot**

<img width="514" height="349" alt="image" src="https://github.com/user-attachments/assets/324bb952-925d-4b0c-bef9-abec62e497ce" />


---

### Program 2: Tracking Nonstationary Bandit with Sliding Window UCB
- Implemented Sliding Window Upper Confidence Bound algorithm
- Simulated nonstationary environment with drifting reward distributions
- Used window size of 50 to adapt to changing reward patterns
- Visualized cumulative rewards showing algorithm's ability to track changing optimal arms
- Demonstrated adaptation to drift parameter (0.2) in 5-armed bandit
  

**Screenshot**

<img width="508" height="386" alt="image" src="https://github.com/user-attachments/assets/d6ff3ccc-5821-49c7-b63b-d7be73478939" />


---

### Program 3: Value Iteration for Markov Decision Process
- Implemented value iteration algorithm for solving MDPs
- Defined 3-state, 2-action environment with transition probabilities
- Used Bellman optimality equation with discount factor (γ=0.9)
- Achieved convergence in 82 iterations with threshold 0.001
- Found optimal policy: [0, 1, 0] for states 0, 1, 2 respectively

**Screenshot**

<img width="547" height="450" alt="image" src="https://github.com/user-attachments/assets/1be93ebb-5fa5-4245-accc-00c9fc4570a4" />


---

### Program 4: Policy Iteration for MDP
- Implemented policy iteration algorithm (alternating evaluation and improvement)
- Created 3-state, 2-action MDP with defined transition probabilities
- Used Bellman expectation equation for policy evaluation
- Found optimal policy: {'s1': 'a2', 's2': 'a2', 's3': 'a1'}
- Achieved state values: s1=24.5, s2=10.5, s3=0.0

**Screenshot**

<img width="479" height="577" alt="image" src="https://github.com/user-attachments/assets/8226dcfb-f5ef-4697-a887-5ac81cf67f7c" />


---

### Program 5: Monte Carlo Methods for Model-Free RL
- Implemented Monte Carlo prediction for Blackjack environment
- Estimated state-value function for random policy over 50,000 episodes
- Implemented Monte Carlo control with epsilon-greedy exploration
- Learned optimal policy for Blackjack decision-making
- Demonstrated model-free learning without transition dynamics

**Screenshot**

<img width="415" height="437" alt="image" src="https://github.com/user-attachments/assets/123bf09a-14b1-4551-8368-d570f0d9ddf4" />
<img width="394" height="207" alt="image" src="https://github.com/user-attachments/assets/7e578d49-ba5a-4fea-a70e-1195632026a4" />
<img width="425" height="578" alt="image" src="https://github.com/user-attachments/assets/61bc06eb-5c9b-4647-ace6-336f83c1f3b9" />


---

### Program 6: Grid World Environment with Random Policy
- Built 4x4 grid world environment with goal state
- Implemented precomputed transition dictionary for efficiency
- Designed reward system: +1 for goal, -0.01 per step
- Created visual rendering with agent (A) and goal (G) markers
- Tested with random policy showing agent movement patterns

**Screenshot**

<img width="571" height="283" alt="image" src="https://github.com/user-attachments/assets/0d2677e7-e444-4678-a061-6dbd26778266" />
<img width="475" height="704" alt="image" src="https://github.com/user-attachments/assets/036e9159-4909-4757-a6fe-481345395a28" />
<img width="469" height="177" alt="image" src="https://github.com/user-attachments/assets/1ddf133b-770e-45a6-943a-eb993a4e3644" />

---

### Program 7: TD(0) Learning with Bootstrapping
- Implemented Temporal Difference learning for 4x4 grid world
- Used TD(0) update rule: V(s) ← V(s) + α[r + γV(s') - V(s)]
- Learned state-value function over 1000 episodes
- Visualized value estimates with heatmap showing gradient toward goal
- Demonstrated bootstrapping concept in reinforcement learning

**Screenshot**

<img width="651" height="464" alt="image" src="https://github.com/user-attachments/assets/66e7047e-b427-47c4-a4a8-a42de2c14a4d" />


---

### Program 8: 1D Grid TD(0) Implementation
- Created simple 1D grid environment with terminal states
- Implemented TD(0) learning with random walk policy
- Learned value function showing progression toward goal state
- Results: State values increase toward terminal reward (+1 at state 5)
- State 2: -0.37, State 3: 0.01, State 4: 0.55 (closest to goal)

**Screenshot**

<img width="512" height="427" alt="image" src="https://github.com/user-attachments/assets/46bf2fd4-f3ad-462b-b91e-672d790e1273" />


---

### Program 9: TD(0) Learning with Obstacles
- Extended grid world with obstacle states (walls)
- Implemented epsilon-greedy TD(0) agent with Q-learning updates
- Trained agent over 500 episodes with obstacle avoidance
- Visualized learning curve showing improvement in rewards
- Tested trained agent showing successful navigation around obstacles

**Screenshot**

<img width="512" height="476" alt="image" src="https://github.com/user-attachments/assets/e05995fd-0746-4c91-b3dc-c28379895183" />
<img width="512" height="540" alt="image" src="https://github.com/user-attachments/assets/b8e4609c-73f6-42de-bee8-ea22957c4d78" />
<img width="534" height="233" alt="image" src="https://github.com/user-attachments/assets/151475d5-a6ea-4297-8f6b-8c5083240036" />

---

### Program 10: Policy Gradient for CartPole
- Implemented REINFORCE policy gradient algorithm
- Built neural network policy with Softmax output
- Used discounted returns with baseline subtraction
- Solved CartPole-v1 environment in 146 episodes
- Achieved target reward of 195+ for 10 consecutive episodes

**Screenshot**

<img width="703" height="308" alt="image" src="https://github.com/user-attachments/assets/93ac6e2a-97d3-4f2a-a082-a5c404f28538" />
<img width="475" height="638" alt="image" src="https://github.com/user-attachments/assets/b882f0a2-18d6-426e-8ca5-1c845ee842ab" />
<img width="612" height="364" alt="image" src="https://github.com/user-attachments/assets/427f11f5-2544-4b4c-91b7-ed5edd26949c" />


