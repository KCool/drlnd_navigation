
# Project 1: Navigation

### Introduction

Train your own DQN agent to navigate in a 3D environment and collect good bananas!

### How it works

The environment is a simplified version of the official Unity [ML Agents](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Learning-Environment-Examples.md#banana-collector) one:

![Banana](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/images/banana.png)

The goal is to collect as many yellow bananas in one episode as possible while avoiding blue bananas. A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana.  

The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around agent's forward direction.  Given this information, the agent has to learn how to best select actions.  Four discrete actions are available, corresponding to:
- **`0`** - move forward.
- **`1`** - move backward.
- **`2`** - turn left.
- **`3`** - turn right.

The task is episodic, and in order to solve the environment, our agent must get an average score of +13 over 100 consecutive episodes.

### Getting Started

1. Set up a python environment including python 3.6+, numpy, matplotlib, torch.

2. Follow the steps in [here](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Installation.md) to install the Unity ML-Agents Toolkit.

3. Clone this repository via `git clone https://github.com/KCool/drlnd_navigation.git`

4. Download the Banana Navigation environment from one of the links below.  Select the environment which matches your operating system:
    - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux.zip)
    - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana.app.zip)
    - Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86.zip)
    - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86_64.zip)
    
5. Place the file in the folder of the repository

If you are still having issues after following this steps regarding the dependencies then please check out the more throughly configuration [here](https://github.com/udacity/deep-reinforcement-learning#dependencies).


### Instructions

Follow the instructions in `Navigation_Solution.ipynb` to train your own agent!

You can also use the pretrained agent `checkpoint_dqn_success.pth` (= pytorch model) which successfully solved the environment (in ~177 steps).
