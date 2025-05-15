# DefenderBench

## Installation

First create a virtual environment and activate it:

    conda create -n defenderbench python=3.10
    conda activate defenderbench

Then install the benchmark:

        pip install .

## Usage

To run the benchmark, use the following script:

    python -m src.examples.run_experiment

For instance, to run the random baseline on all the environments/tasks

    python -m src.examples.run_experiment --llm random

To manually run a specific environment/task

    python -m src.examples.run_experiment --llm human --env_name CyberBattleChain10

To list all the available environments/tasks and additional settings use:

    python -m src.examples.run_experiment --help

## Usage using a custom agent

Here's a simple example of an actor-critic multi-agent architecture

    python agents/actor_critic.py

## Contributing

This project welcomes contributions and suggestions.