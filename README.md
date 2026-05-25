# Implementation of SARSA Control Algorithm using FrozenLake Environment

## Aim

To implement the SARSA (State-Action-Reward-State-Action) Control algorithm for learning the optimal policy in the FrozenLake environment using Reinforcement Learning.

---

## Algorithm

### SARSA Control Algorithm

1. Import the required libraries.
2. Create the FrozenLake environment using OpenAI Gym.
3. Initialize:
   - Learning rate \( \alpha \)
   - Discount factor \( \gamma \)
   - Exploration rate \( \epsilon \)
   - Q-table \( Q(s,a) \)
4. Define the epsilon-greedy policy:
   - Choose a random action with probability \( \epsilon \).
   - Otherwise choose the action with the highest Q-value.
5. For each episode:
   - Reset the environment.
   - Choose an initial action using the epsilon-greedy policy.
   - Repeat until the episode ends:
     - Take the selected action.
     - Observe:
       - Next state
       - Reward
       - Terminal condition
     - Select the next action using the epsilon-greedy policy.
     - Update the Q-value using SARSA update rule:

\[
Q(s,a) \leftarrow Q(s,a) + \alpha \left[
r + \gamma Q(s',a') - Q(s,a)
\right]
\]

     - Update the current state and action.
6. Store rewards for each episode.
7. Reduce epsilon gradually for better exploitation.
8. Display the learned Q-table and reward performance graph.

---

## Program

```python


      
```

---

## Output

```text

```

---

## Output Graph

The graph shows the reward obtained per episode during SARSA training. As training progresses, the rewards increase, indicating that the agent learns the optimal policy.

---

## Result

Thus, the SARSA Control algorithm was successfully implemented in the FrozenLake environment. The agent learned the optimal action-value function and improved its performance through continuous interaction with the environment using on-policy Temporal Difference learning.
