# Snake Game Environment Using OpenAI

This is a project I completed as part of the "Practical AI with Python and Reinforcement Learning" Udemy course. The goal of the project was to create a Snake game environment using the OpenAI Gym library, which allows developers to create custom environments for training and testing reinforcement learning algorithms.

## Installation

To use this Snake game environment, follow these steps:

1. Clone the repository:

```bash
git clone https://github.com/username/snake-game-environment.git
```

2. Install the necessary dependencies:

```bash
pip install gym numpy pygame
```

## Usage

To use the Snake game environment, simply import the `SnakeEnv` class from the `snake_env.py` file:

```python
from snake_env import SnakeEnv

env = SnakeEnv()
```

The `SnakeEnv` class inherits from the OpenAI `gym.Env` class, so you can use it in the same way as any other OpenAI environment. For example, to reset the environment and get the initial state:

```python
obs = env.reset()
```

And to take an action in the environment:

```python
action = 0  # replace with your chosen action
obs, reward, done, info = env.step(action)
```

The `step` method returns four values:

- `obs`: the new observation (state) after taking the action
- `reward`: the reward for taking the action
- `done`: a boolean indicating whether the episode is over (i.e., the Snake has died or won)
- `info`: any additional information about the environment

## Customization

If you want to customize the Snake game environment, you can modify the `snake_env.py` file. Some possible modifications include:

- Changing the size of the game window and the Snake
- Modifying the reward function
- Adding additional actions or observations
- Changing the game rules (e.g., the Snake's movement speed)

## Acknowledgements

This project was completed as part of the "Practical AI with Python and Reinforcement Learning" Udemy course, which provided guidance on how to create the Snake game environment using OpenAI Gym. The `snake_env.py` file is based on the code provided in the course.