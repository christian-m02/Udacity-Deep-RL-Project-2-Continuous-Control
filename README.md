[//]: # (Image References)

[image1]: https://user-images.githubusercontent.com/10624937/43851024-320ba930-9aff-11e8-8493-ee547c6af349.gif "Trained Agent"
[image2]: https://user-images.githubusercontent.com/10624937/43851646-d899bf20-9b00-11e8-858c-29b5c2c94ccc.png "Crawler"

This project is part of Udacity's Nanodegree on Deep Reinforcement Learning (https://eu.udacity.com/course/deep-reinforcement-learning-nanodegree--nd893).


# Project 2: Continuous Control

### Introduction

For this project, I will work with the [Reacher](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Learning-Environment-Examples.md#reacher) environment which uses the Unity Machine Learning Agents Toolkit (https://github.com/Unity-Technologies/ml-agents)
, an open-source Unity plugin.


![Trained Agent][image1]

In this environment, a double-jointed arm can move to target locations. A reward of +0.1 is provided for each step that the agent's hand is in the goal location. 

Goal of the exercise is to train an agent via Reinforcement Learning to maintain its position at the target location for as many time steps as possible.

The observation space consists of 33 variables corresponding to position, rotation, velocity, and angular velocities of the arm. Each action is a vector with four numbers, corresponding to torque applicable to two joints. Every entry in the action vector should be a number between -1 and 1.

For this project, two separate versions of the Unity environment are provided:
- The first version contains a single agent.
- The second version contains 20 identical agents, each with its own copy of the environment.  

I have used the single agent version of the Unity environment.

The task is episodic, and in order to solve the environment, the agent must get an average score of +30 over 100 consecutive episodes.

The ipython notebook `Parameter_Study.ipynb` contains the study of the hyperparameters of the DDPG Agent for performing this
task. Two successful DDPG agents along with their respective hyperparameter settings are given in `Continuous_Control.ipynb`.
For a discussion of the findings and assessment of the agents see the Report.pdf.



# Prerequisites

Running this notebook requires Python 3.5 (or higher), the Reacher environment (see below) and the following Python libraries:

- NumPy
- PyTorch
- Unity Machine Learning Agents Toolkit
- OpenAI Gym



# To get started -

Below are the instructions on how to get started on this project as given in the original repository.
The original repository can be found here: https://github.com/udacity/deep-reinforcement-learning/tree/master/p2_continuous-control



### Getting Started

1. Download the environment from one of the links below.  You need only select the environment that matches your operating system:

    - **_Version 1: One (1) Agent_**
        - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Linux.zip)
        - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher.app.zip)
        - Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Windows_x86.zip)
        - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Windows_x86_64.zip)
    

    (_For AWS_) If you'd like to train the agent on AWS (and have not [enabled a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md)), then please use [this link](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Linux_NoVis.zip) to obtain the "headless" version of the environment.  You will **not** be able to watch the agent without enabling a virtual screen, but you will be able to train the agent.  (_To watch the agent, you should follow the instructions to [enable a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md), and then download the environment for the **Linux** operating system above._)

2. Place the file in the DRLND GitHub repository, in the `Udacity-Deep-RL-Project-2-Continuous-Control/` folder, and unzip (or decompress) the file. 

