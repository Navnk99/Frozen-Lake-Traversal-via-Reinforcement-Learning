# Frozen-Lake-Traversal-via-Reinforcement-Learning with 8x8 Grid

This repository contains code for solving the Frozen Lake environment using reinforcement learning techniques. The Frozen Lake environment is a classic problem in reinforcement learning, often used for educational purposes.

## Contents

- `FrozenLake`: A Jupyter notebook containing the implementation and explanation of reinforcement learning algorithms applied to the Frozen Lake environment.
- `frozen_lake.py`: Python script defining the Frozen Lake environment, including functions for generating random maps and rendering the environment.

## Environment Description

The Frozen Lake environment consists of a grid where each cell can be:

- **S**: Starting point, safe
- **F**: Frozen surface, safe
- **H**: Hole, fall to your doom
- **G**: Goal, where the frisbee is located

The objective is to navigate from the starting point to the goal without falling into any holes. The ice is slippery, so the agent won't always move in the intended direction.

### Example Grids

**4x4 Grid:**
SFFF
FHFH
FFFH
HFFG

**8x8 Grid:**
SFFFFFFF
FFFFFFFF
FFFHFFFF
FFFFFHFF
FFFHFFFF
FHHFFFHF
FHFFHFHF
FFFHFFFG

## Files Description

### `FrozenLakeTraversal_via_Reinforcement_Learning.ipynb`

This notebook demonstrates the application of reinforcement learning algorithms to solve the Frozen Lake environment. It includes:

- Initialization of the Frozen Lake environment.
- Implementation of various reinforcement learning algorithms such as Q-learning and SARSA.
- Visualization of the agent's performance and learned policy.

### `frozen_lake.py`

This script defines the Frozen Lake environment, including:

- **FrozenLakeEnv Class**: Defines the Frozen Lake environment and its dynamics.
- **generate_random_map Function**: Generates a random valid map with a path from the start to the goal.
- **render Function**: Provides a way to visualize the environment.

## Dependencies

The following dependencies are required to run the code:

- Python 3.x
- NumPy
- Gym
- Six

You can install the required packages using pip:
pip install numpy gym six

## Usage

To run the notebook, simply open it in Jupyter Notebook or Jupyter Lab and execute the cells sequentially. The notebook provides detailed explanations and visualizations to help you understand the reinforcement learning process.

License
This project is licensed under the MIT License. See the LICENSE file for more details.

Acknowledgments
This project is inspired by OpenAI's Gym environments and the educational materials on reinforcement learning.

To use the `frozen_lake.py` script, you can import the `FrozenLakeEnv` class into your Python code and create an instance of the environment:

```python
from frozen_lake import FrozenLakeEnv
env = FrozenLakeEnv(map_name="4x4", is_slippery=True)
env.reset()
env.render()

