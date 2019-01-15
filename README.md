[//]: # (Image References)

[image1]: https://user-images.githubusercontent.com/10624937/42135619-d90f2f28-7d12-11e8-8823-82b970a54d7e.gif "Trained Agent"

# Banana navigation

## Deep Reinforcement Learning Nanodegree, Udacity

@rtbins

## Synopsis

In this project, an agent is trained to navigate (and collect bananas!) in a large, square world. The implemetation of agent uses Deep q networks.

![Trained Agent][image1]

A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana.  Thus, the goal of the agent is to collect as many yellow bananas as possible while avoiding blue bananas.  

The state space has `37 dimensions` and contains agent's velocity, along with ray-based perception of objects around agent's forward direction.  Given this information, the agent has to learn how to best select actions.  Four discrete actions are available, corresponding to:

- **`0`** - move forward.
- **`1`** - move backward.
- **`2`** - turn left.
- **`3`** - turn right.

The task is episodic, and in order to solve the environment, an agent must get an average score of `+13` over `100` consecutive episodes.

## Getting started

1. Request and download the environment from Udacity. These environments are specific to OS. 
2. Place the file in the root folder and unzip (or decompress) the file.

3. Create (and activate) a new environment with Python 3.6.

- __Linux__ or __Mac__: 

```bash
conda create --name drlnd python=3.6
source activate drlnd
```

- __Windows__: 

```bash
conda create --name drlnd python=3.6 
activate drlnd
```

4. Clone the repository, and navigate to the `python/` folder.  Then, install several dependencies.

```bash
git clone https://github.com/udacity/deep-reinforcement-learning.git
cd deep-reinforcement-learning/python
pip install .
```

5. Create an [IPython kernel](http://ipython.readthedocs.io/en/stable/install/kernel_install.html) for the `drlnd` environment. 

```bash
python -m ipykernel install --user --name drlnd --display-name "drlnd"
```

6. Before running code in a notebook, change the kernel to match the `drlnd` environment by using the drop-down `Kernel` menu.

## Instructions

The project consists of 5 files

- Navigation.ipynb - this is jupyter notebook containing all analysis.
- agent.py - contains the implementation for a DQN agent
- model.py - the neural net model
- navigation-checkpoint.pth - saved trained model (pytorch)
- Report.md - description for the implementation.