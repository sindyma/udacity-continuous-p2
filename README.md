# udacity-continuous-p2
Project 2: Continuous Control for Udacity's Deep Reinforcement Learning Nanodegree. This repo contains a project to meet requirements for the Udacity Reinforcement Learning Nanodegree.

# Background
This is the second coding project in [Udacity's Deep RL nanodegree](https://www.udacity.com/course/deep-reinforcement-learning-nanodegree--nd893). Prior to this project, the degree takes you through reinforcement learning theory first and then moves onto deep RL.  We are tasked to solve a modified Reacher (unity ML) environment, scoring 30 or more over 100 episodes. To solve this environment, I have chosen to follow the benchmark implementation and use DDPG on the 2nd version of the environment that trains on 20 agents simulatenously.

# Getting started
To get started, download the training environment for your OS:

* Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux.zip)

* Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana.app.zip)

* Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86.zip)

* Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86_64.zip)

Next, clone this github repo:

```git clone https://github.com/sindyma/udacity-continuous-p2.git```

Before running the Jupyter Notebook, ensure all requirements are installed. To do this, navigate to the cloned repo and run the following command. This will install all packages specified in `requirements.txt`.

```pip install .```

Open Continuous_Control_20_Agents.ipynb in the root directory. This Jupyter Notebook uses an actor-critic algorithm to train 20 agents simultaneously.

# Troubleshooting
If you aren't able to get started, see if any of the following describe your situation:
* Python version
This repo has been developed with python 3.7. Python 2 users may need to switch their kernel and ensure all dependencies have been installed for python 3.7
* Dependencies
You may need to install dependencies:
* unity-ml
* numpy
* torch
* matplotlib

# The environment and success criteria
* The state space in this environment has 33 dimensions: position, rotation, velocity, and angular velocities of the two arm Rigidbodies.
* The action space is continuous and of size 4, corresponding to torque applicable to two joints.
* The reward function is: +0.1 Each step agent's hand is in goal location.

In order to solve the environment, the 20 agents need to get an average score of 30 over 100 episodes.

# Part 1: Training
Follow the markdown instructions in `Continuous_Control_20_Agents.ipynb` to train your own agent. At the end of training, your weights will be saved in the folder in two .pth files (one for the actor and one for the critic). If these files exist from a previous training session, this will be overwritten.

# Part 2: Run a trained agent
The final section in `Continuous_Control_20_Agents.ipynb` runs a trained agent (submission for the project).

# Troubleshooting
If you aren't able to get started, see if any of the following describe your situation:
* Python version
This repo has been developed with python 3.7. Python 2 users may need to switch their kernel and ensure all dependencies have been installed for python 3.7
* Dependencies
You may need to install dependencies:
* unity-ml
* numpy
* torch
* matplotlib
