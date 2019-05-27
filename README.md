# Simple pytorch implmentation of reinforcement learning algorithms

This repository is for those who want to implement the RL algorithms after reading the corresponding papers.
All the algorithms are encapsulated in one file as minimum working examples, which let you focus more on the algorithm themselves.
## Requirements:
- python>=3.5
- pytorch>=0.4.0
- gym
- drawnow



## 1. DQN
#### Discrete action space: CartPole-v0:
<img src="https://github.com/zzzxxxttt/pytorch_rl_iof/blob/master/figures/dqn_cartp.png" width="500" />

- Code mainly adopted from https://pytorch.org/tutorials/intermediate/reinforcement_q_learning.html

## 2. REINFORCE
#### Discrete action space: CartPole-v0:
<img src="https://github.com/zzzxxxttt/pytorch_rl_iof/blob/master/figures/reinforce_cartp.png" width="500" />

- Code mainly adopted from https://github.com/JamesChuanggg/pytorch-REINFORCE

## 3. A2C
#### Discrete action space: CartPole-v0:
<img src="https://github.com/zzzxxxttt/pytorch_rl_iof/blob/master/figures/a2c_cartp.png" width="500" />

#### Continuous action space: MountainCarContinuous-v0:
<img src="https://github.com/zzzxxxttt/pytorch_rl_iof/blob/master/figures/a2c_mtcar.png" width="500" />

- Code mainly adopted from https://gist.github.com/Ashioto/10ec680395db48ddac1ad848f5f7382c#file-actorcritic-py
- I just rewrite the code using pytorch. As mentioned by the original author, this a2c code is extremely unstable, if you find it does not work, just kill the process and restart training :)

## 4. DDPG
#### Continuous action space: MountainCarContinuous-v0:
<img src="https://github.com/zzzxxxttt/pytorch_rl_iof/blob/master/figures/ddpg_mtcar.png" width="500" />

- Code mainly adopted from https://github.com/lirnli/OpenAI-gym-solutions/blob/master/Continuous_Deep_Deterministic_Policy_Gradient_Net/DDPG%20Class%20ver2.ipynb
- I just rewrite the code using pytorch, and fixed a small bug in the original code when updating the actor.

## 5. DDPG with Prioritized Experience Replay
#### Continuous action space: MountainCarContinuous-v0:
<img src="https://github.com/zzzxxxttt/pytorch_rl_iof/blob/master/figures/ddpg_per_mtcar.png" width="500" />

- In the original paper, the prioritized experience replay is implemented using binary heap for efficient training.
Due to the small buffer size in our toy example, I just use an array to store samples and sort it after every update.

## 6. TRPO
#### Continuous action space: MountainCarContinuous-v0:
<img src="https://github.com/zzzxxxttt/pytorch_rl_iof/blob/master/figures/trpo_mtcar.png" width="500" />

- Code mainly adopted from https://github.com/ikostrikov/pytorch-trpo
- This piece of code is a little bit complicated, I've tried my best to place everything (LBFGS, conjugate gradient, line search, GAE, ...) in one file.
- ~ 300 lines, not so horrible, right?

## 7. PPO
#### Continuous action space: MountainCarContinuous-v0:
<img src="https://github.com/zzzxxxttt/pytorch_rl_iof/blob/master/figures/ppo_mtcar.png" width="500" />

- Code mainly adopted from https://github.com/tpbarron/pytorch-ppo

## 8. ACER
#### Discrete action space: CartPole-v0:
<img src="https://github.com/zzzxxxttt/pytorch_rl_iof/blob/master/figures/acer_cartp.png" width="500" />

- Code mainly adopted from https://github.com/dchetelat/acer

