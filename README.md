# HNN-RAN3SAT-T2Fuzzy-AFSA Framework

**Interval Type-2 Fuzzy Random 3-SAT Representation in Third-Order Hopfield Networks with AFSA Optimization for Uncertainty-Aware Classification in Digital Finance**

## 1. Overview

This repository contains the computational framework developed for the study of uncertainty-aware classification in digital finance using an integrated approach based on Interval Type-2 Fuzzy (IT2F) modelling, Random 3-SAT (RAN3SAT) representation, Third-Order Hopfield Neural Networks (HNNs), and Artificial Fish Swarm Algorithm (AFSA) optimization.

The proposed HNN-RAN3SAT-T2Fuzzy-AFSA framework is designed to address uncertainty, complex feature interactions, and classification challenges in digital financial data. It combines fuzzy representation and higher-order neural computation with metaheuristic optimization to support the identification of complex patterns associated with financial risk and anomalous transactions.

The framework is evaluated using **both simulated data and real-world digital financial datasets**. Simulated data provide controlled experimental conditions for investigating the behaviour of the proposed method under different levels of uncertainty, noise, and data complexity. Real-world datasets are used to assess its practical performance in financial fraud detection, lending-risk prediction, and cryptocurrency transaction anomaly detection.

The main objectives of the repository are to:

- Provide the computational implementation of the proposed framework.
- Support the experimental evaluation reported in the associated study.
- Facilitate reproducibility through documented experimental settings and random seeds.
- Enable further research on fuzzy logic, higher-order neural networks, and uncertainty-aware financial classification.

## 2. Repository Contents

The repository is organised to separate the implementation, datasets, experimental procedures, and evaluation outputs.

```text
HNN-RAN3SAT-T2Fuzzy-AFSA-framework/
│
├── README.md
├── LICENSE
├── CITATION.cff
├── requirements.txt
├── pyproject.toml
│
├── src/
│   ├── fuzzy/
│   │   └── interval_type2_fuzzy.py
│   │
│   ├── logic/
│   │   └── random_3sat.py
│   │
│   ├── networks/
│   │   └── third_order_hopfield.py
│   │
│   ├── optimization/
│   │   └── afsa.py
│   │
│   ├── classification/
│   │   └── classifier.py
│   │
│   └── evaluation/
│       └── metrics.py
│
├── data/
│   ├── simulated/
│   └── real_world/
│
├── experiments/
│   ├── simulated_data_experiments.py
│   ├── credit_card_fraud.py
│   ├── lendingclub_default.py
│   └── elliptic_anomaly_detection.py
│
├── results/
│   ├── simulated/
│   └── real_world/
│
├── figures/
│
├── pseudocode/
│
├── reproducibility/
│   ├── random_seeds.txt
│   ├── environment.txt
│   └── experimental_settings.md
│
└── tests/
```

*Note: This structure describes the intended organisation of the project. The actual directory and file names should be kept consistent with the files uploaded to the repository.*

## 3. Computational Framework

The proposed framework integrates six principal computational components:

1. **Interval Type-2 Fuzzy Modelling:** Represents uncertainty in input features through interval type-2 fuzzy sets, allowing the model to accommodate imprecision and variability in financial observations.

2. **Random 3-SAT Representation:** Encodes the relevant classification structure using random 3-SAT formulations, providing a logical representation for modelling complex relationships among input variables.

3. **Third-Order Hopfield Neural Network:** Uses higher-order interactions to represent complex dependencies among variables and support the computational processing of the logical representation.

4. **Artificial Fish Swarm Algorithm:** Optimizes the relevant model parameters and network configurations through a population-based metaheuristic search procedure.

5. **Digital Financial Classification:** Applies the integrated framework to financial classification tasks, including fraud detection, lending-default prediction, and cryptocurrency transaction anomaly detection.

6. **Performance Evaluation:** Assesses predictive performance using appropriate classification metrics and comparative experimental analysis.

## 4. Datasets

The experimental evaluation uses two complementary data sources: simulated datasets and publicly available real-world digital financial datasets.

### 4.1 Simulated Data

Simulated datasets are generated to investigate the behaviour of the proposed framework under controlled experimental conditions. They allow systematic examination of the effects of uncertainty, noise, feature interactions, and data complexity on classification performance.

The simulation procedures, parameter settings, and data-generation assumptions should be documented alongside the corresponding experimental scripts. This enables the simulated experiments to be reproduced independently and provides a controlled basis for analysing the framework's computational behaviour.

### 4.2 Real-World Digital Financial Data

The proposed framework is also evaluated using the following publicly available datasets:

| Dataset | Application | Source |
|---|---|---|
| Credit Card Fraud Detection | Financial fraud detection | [Kaggle dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud) |
| Peer-to-Peer Lending Default Prediction (LendingClub) | Loan-default and credit-risk prediction | [Kaggle dataset](https://www.kaggle.com/datasets/wordsforthewise/lending-club) |
| Cryptocurrency Transaction Anomaly Detection (Elliptic) | Cryptocurrency transaction anomaly detection | [Kaggle dataset](https://www.kaggle.com/datasets/ellipticco/elliptic-data-set) |

These datasets provide different digital financial classification scenarios, allowing the framework to be evaluated across fraud detection, credit-risk assessment, and cryptocurrency transaction analysis.

The datasets are obtained from their respective public sources rather than redistributed in this repository unless their licensing conditions permit redistribution. Users should consult the original dataset pages for access requirements, licensing information, and documentation.

### 4.3 Data Preprocessing

Data preprocessing should follow the procedures specified in the study. Depending on the dataset, these may include:

- Handling missing or inconsistent observations.
- Encoding categorical variables where necessary.
- Scaling or normalising numerical features.
- Defining the target classification labels.
- Applying feature-selection procedures.
- Splitting the data into training, validation, and testing subsets.

All preprocessing operations should be performed consistently across the proposed method and comparison models. Any resampling, feature selection, or parameter estimation should be conducted using the training data only, where applicable, to minimise data leakage.

## 5. Reproducibility Protocol

The experiments are designed to support reproducible evaluation of the proposed HNN-RAN3SAT-T2Fuzzy-AFSA framework.

The reproducibility protocol covers:

- Random seed settings.
- Data-generation parameters for simulated experiments.
- Data preprocessing and feature-selection procedures.
- Model architecture and parameter configurations.
- AFSA optimization settings.
- Training, validation, and testing procedures.
- Computational environment and software dependencies.
- Per-run experimental outputs.

Where multiple independent runs are performed, the random seeds and individual run results should be retained and reported. If the study uses 30 independent runs, the corresponding seed values and outputs should be included in the repository to support verification of the reported mean and standard deviation.

The exact seeds, environment specifications, per-run result files, and feature-selection indices described in Section~\ref{subsec:reproducibility} should be included in the final repository release.

## 6. Experimental Framework

The experimental evaluation is organised around two complementary settings.

### 6.1 Experiments Using Simulated Data

The simulated-data experiments examine the computational and classification behaviour of the proposed framework under controlled conditions. They provide an opportunity to investigate how changes in uncertainty, noise, and data complexity influence model performance.

### 6.2 Experiments Using Real-World Financial Data

The real-world experiments evaluate the framework on three digital financial classification tasks:

- Credit card fraud detection.
- Peer-to-peer lending default prediction.
- Cryptocurrency transaction anomaly detection.

These experiments assess the applicability of the proposed approach to different financial data structures and classification problems.

### 6.3 Performance Metrics

The evaluation may include the following metrics, depending on the classification task and the experimental design:

- Accuracy
- Precision
- Recall
- F1-score
- Matthews Correlation Coefficient (MCC)
- Area Under the Receiver Operating Characteristic Curve (ROC-AUC)

For imbalanced financial classification problems, particular attention should be given to precision, recall, F1-score, MCC, and ROC-AUC rather than relying exclusively on accuracy.

All reported metrics should be calculated using the same evaluation protocol for the proposed framework and the baseline methods. The repository should retain the underlying outputs required to verify the reported experimental results.

## 7. Installation and Execution

### 7.1 Requirements

The framework is implemented in Python. The required packages and their versions should be specified in `requirements.txt` or `pyproject.toml`.

### 7.2 Installation

Clone the repository:

```bash
git clone https://github.com/zeeham4u2c/HNN-RAN3SAT-T2Fuzzy-AFSA-framework.git
cd HNN-RAN3SAT-T2Fuzzy-AFSA-framework
```

Create and activate a virtual environment:

```bash
python -m venv venv
```

On Windows:

```bash
venv\Scripts\activate
```

On Linux or macOS:

```bash
source venv/bin/activate
```

Install the dependencies:

```bash
pip install -r requirements.txt
```

### 7.3 Running the Experiments

The experiment scripts should be executed according to the actual filenames and instructions provided in the repository.

For example, if the corresponding scripts are included:

```bash
python experiments/simulated_data_experiments.py
python experiments/credit_card_fraud.py
python experiments/lendingclub_default.py
python experiments/elliptic_anomaly_detection.py
```

The commands above illustrate the intended experiment organisation. They should be adjusted to match the scripts included in the final repository.

## 8. Random Seeds and Experimental Settings

Random seeds are used to support reproducibility, particularly in experiments involving stochastic optimisation, random data generation, and neural-network initialisation.

The seed values, parameter configurations, and experimental settings should be documented in the `reproducibility/` directory. Where the study reports results over multiple independent runs, the repository should include the corresponding run-level outputs.

The final release should ensure that:

- The reported random seeds match those used in the experiments.
- The simulation parameters match the data-generation procedures.
- The AFSA settings match the optimisation procedure described in the manuscript.
- The network architecture and learning parameters match the reported model.
- The feature-selection indices correspond to those used in the reported experiments.
- The saved results can be traced to the relevant experiment scripts.

## 9. Code Availability

The source code for the proposed HNN-RAN3SAT-T2Fuzzy-AFSA framework is available at:

**GitHub repository:**  
https://github.com/zeeham4u2c/HNN-RAN3SAT-T2Fuzzy-AFSA-framework

The repository provides the computational implementation and experimental resources associated with the study. A permanent archived version and Zenodo DOI will be registered upon acceptance of the manuscript.

The real-world datasets are accessible through the original public sources listed in Section 4. The simulated datasets can be regenerated using the documented data-generation procedures, provided that the relevant scripts and parameter settings are included in the final release.

## 10. Citation

If you use this framework in your research, please cite the associated publication after its bibliographic details become available.

A suggested citation format is:

Abubakar, H. et al. (Year).
Interval Type-2 Fuzzy Random 3-SAT Representation in Third-Order
Hopfield Networks with AFSA Optimization for Uncertainty-Aware
Classification in Digital Finance.
[Journal Name], [Volume(Issue)], [Page Range].
DOI: [To be added].


A `CITATION.cff` file may also be included to provide machine-readable citation metadata.




