# Low-Carbon Commuting Adoption Simulation

This repository contains the notebook and final report for a computational modelling project about low-carbon commuting adoption.

## Research Question

Does targeting central individuals lead to higher adoption of low-carbon commuting than targeting random initial adopters in a social network simulation?

## Project Description

This project uses a simple agent-based simulation. Each person is represented as a node in a social network. Some people adopt low-carbon commuting at the start, and other people adopt later if enough of their connected people have already adopted.

The project compares two starting strategies:

1. Random targeting: initial adopters are selected randomly.
2. Central targeting: initial adopters are selected from the most connected people in the network.

## Model Setup

- Number of agents: 1,000
- Network type: scale-free network
- Initial adopters: 5%
- Adoption thresholds tested: 0.1, 0.2, 0.3, 0.4, 0.5
- Repetitions: 100 per condition
- Strategies compared: random targeting and central targeting

## Main Finding

The results show that central targeting works better when adoption requires moderate or strong social influence. At low thresholds, both strategies reach high adoption. At higher thresholds, random targeting often stops early, while central targeting produces much higher adoption.

## Files

- `low_carbon_commuting_simulation.ipynb`: notebook with code, explanations, results, and plots.
- `low_carbon_commuting_final_report.pdf`: final report.

## How to Run

Open the notebook in Google Colab or Jupyter Notebook and run the cells from top to bottom.

Required Python packages:

```python
networkx
pandas
matplotlib
