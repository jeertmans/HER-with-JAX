# Learning Hindsight Experience Replay with JAX

This small repository provides a minimal JAX implementation of the bit-flipping experiment presented in the paper Hindsight Experience Replay (https://arxiv.org/abs/1707.01495).

The authors provide a PyTorch implementation, which this implementation draws inspiration from; see https://github.com/hemilpanchiwala/Hindsight-Experience-Replay.

Following JAX's design philosophy, everything is written in a functional programming style, which, in my opinion, makes the code much easier to follow.

## Installing

The project dependencies are listed in the `pyproject.toml` file. You can install them using `pip`:

```bash
pip install .
```

If you want to install JAX with CUDA support, use the following command:

```bash
pip install . --group cuda
```

Note that the `pyproject.toml` adheres to the [PEP 621](https://peps.python.org/pep-0621/) and [PEP 735](https://peps.python.org/pep-0735/) guidelines, so any modern Python package manager should be able to correctly install the dependencies.

## Running locally

To run the experiment locally, you also need JupyterLab (or Jupyter Notebook) installed. You can do this by running:

```bash
pip install . --group jupyterlab
```

Then, you can start JupyterLab with the following command:

```bash
jupyter lab
```

## Running on Colab

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/jeertmans/HER-with-JAX/blob/main/bit_flipping.ipynb)

## Contributing

This project aims to keep the code small and clean. However, any contribution regarding:
- bug fixes;
- documentation typos;
- or any mismatch with the original model;

is more than welcome!
