# HNN-RAN3SAT-T2Fuzzy-AFSA-framework
Reproducibility codes for Interval Type-2 Fuzzy Random 3-SAT Representation in Third-Order Hopfield Networks with AFSA Optimization for Uncertainty-Aware Classification in Digital Finance
# Interval Type-2 Fuzzy Random 3-SAT Representation in Third-Order Hopfield Networks with AFSA Optimization for Uncertainty-Aware Classification in Digital Finance

## Overview

This repository contains the computational implementation and supplementary materials for the research paper entitled:

**Interval Type-2 Fuzzy Random 3-SAT Representation in Third-Order Hopfield Networks with AFSA Optimization for Uncertainty-Aware Classification in Digital Finance.**

The study develops an uncertainty-aware classification framework based on an Interval Type-2 Fuzzy Random 3-SAT representation embedded in Third-Order Hopfield Networks (HNNs), with Artificial Fish Swarm Algorithm (AFSA) optimization.

The repository is intended to support the transparency, verification, and reproducibility of the proposed mathematical framework and its computational experiments.

## Repository Contents

- `src/`: Core implementation of the proposed mathematical framework.
- `algorithms/`: Third-order Hopfield network and AFSA optimization algorithms.
- `data/`: Experimental datasets or instructions for obtaining the data.
- `experiments/`: Experimental configurations and classification procedures.
- `results/`: Numerical outputs, performance metrics, and experimental results.
- `figures/`: Scripts and instructions for reproducing manuscript figures.
- `pseudocode/`: Pseudocode and algorithmic descriptions.
- `reproducibility/`: Random seeds, tuning protocols, initialization settings, data splits, and experimental configurations.
- `requirements.txt`: Software dependencies.

## Reproducibility Protocol

The experiments use random seeds 1–30 to govern AFSA initialization, Hopfield network update order, and data splitting, as specified in the manuscript.

The repository provides the implementation codes, pseudocode, parameter-tuning protocols, preprocessing procedures, and figure-reproduction instructions required to reproduce the computational experiments.

## Experimental Framework

The computational implementation covers:

1. Interval Type-2 Fuzzy Random 3-SAT representation.
2. Third-Order Hopfield Network formulation and update procedures.
3. Artificial Fish Swarm Algorithm optimization.
4. Uncertainty-aware digital finance classification.
5. Experimental evaluation and performance assessment.
6. Reproduction of the numerical results and figures reported in the manuscript.

## Installation and Execution

Clone the repository:

```bash
git clone https://github.com/HNN-RAN3SAT-T2Fuzzy-AFSA/framework.git
cd framework
```

Install the required dependencies:

```bash
pip install -r requirements.txt
```

Run the relevant experimental scripts using the instructions provided in their respective directories.

## Random Seeds and Experimental Settings

The random seeds 1–30 are used to support repeated experimental runs and reproducibility. The corresponding initialization, update-order, and data-splitting configurations are documented in the `reproducibility/` directory.

## Code Availability

All research codes and supplementary computational materials are made available through this public repository:

https://github.com/HNN-RAN3SAT-T2Fuzzy-AFSA/framework

## Citation

Please cite the associated research article when using this implementation or its computational materials.
