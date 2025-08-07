# Reinforcement Learning for BabyAI

This project implements reinforcement learning agents for the [BabyAI platform](https://github.com/mila-iqia/babyai), a research environment for grounded language learning with a focus on sample efficiency.

## Features

- Training RL agents on BabyAI levels
- Evaluation and logging
- Customizable agent architectures

## Dependencies

Before running the code, ensure you have the following dependencies installed:

- Python 3.7+
- [BabyAI](https://github.com/mila-iqia/babyai)
- torch (PyTorch)
- numpy
- gym
- tqdm
- matplotlib (for plotting, optional)


## Setup

1. Clone this repository:

2. Install the dependencies as described above.

## Running Training

To train an agent on a BabyAI level, run:

```bash
python train.py --env <BabyAI-level> --algo <algorithm> --episodes <num_episodes>
```

Example:

```bash
python train.py --env BabyAI-GoToLocal-v0 --algo ppo --episodes 10000
```

- `--env`: Name of the BabyAI environment (e.g., `BabyAI-GoToLocal-v0`)
- `--algo`: RL algorithm to use (e.g., `dqn`, `ppo`)
- `--episodes`: Number of training episodes

## Evaluation

To evaluate a trained agent:

```bash
python evaluate.py --env <BabyAI-level> --model-path <path_to_model>
```

## Project Structure

- `train.py`: Script to train RL agents.
- `evaluate.py`: Script to evaluate trained agents.
- `models/`: Contains model definitions.
- `utils/`: Utility functions and helpers.

## Notes

- Make sure the BabyAI environments are registered and available.
- For more details on BabyAI levels and tasks, refer to the [BabyAI documentation](https://github.com/mila-iqia/babyai).

## License

This project is for research and educational purposes.

