## Super-Mario-RL 

**This is a private project to make Super Mario Agent.**

It consists of training an agent to clear Super Mario Bros with deep reinforcement learning methods.

<p float="center">
  <img src="/mario1.gif" width="350" />
  <img src="/mario14.gif" width="350" /> 
</p>

## Project Structure
**main.py**
Main loop between Environment and Mario

**agent.py**
Define how the agent collects experiences, makes actions given observations and updates the action policy.

**wrappers.py**
Environment pre-processing logics, including observation resizing, rgb to grayscale, etc.

**neural.py**
Define Q-value estimators backed by a convolution neural network.

**metrics.py**
Define a `MetricLogger` that helps track training/evaluation performance.

**tutorial.ipynb**
Interactive tutorial with extensive explanation and feedback.

## Key Metrics

- Episode: current episode
- Step: total number of steps Mario played
- Epsilon: current exploration rate
- MeanReward: moving average of episode reward in past 100 episodes
- MeanLength: moving average of episode length in past 100 episodes
- MeanLoss: moving average of step loss in past 100 episodes
- MeanQValue: moving average of step Q value (predicted) in past 100 episodes
