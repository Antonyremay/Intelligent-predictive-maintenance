# Intelligent Predictive Maintenance System

An end-to-end Machine Learning project focused on predicting turbofan engine failure risk and estimating Remaining Useful Life (RUL) using NASA's C-MAPSS dataset.

## Project Overview

Unexpected engine failures can lead to equipment downtime, maintenance costs, and operational risks. Predictive maintenance uses historical sensor measurements and machine learning techniques to identify potential failures before they occur.

This project aims to develop a predictive maintenance system that analyses turbofan engine sensor data to estimate engine health and predict remaining useful life.

## Project Objectives

The project focuses on two primary machine learning tasks:

1. **Engine Failure Risk Classification:** Classify whether an engine is approaching failure based on its estimated Remaining Useful Life (RUL). The planned high-risk threshold is RUL ≤ 30 cycles.
2. **Remaining Useful Life Prediction:** Predict the number of operational cycles remaining before an engine reaches its simulated failure point.

## Dataset

- **Dataset:** NASA C-MAPSS (Commercial Modular Aero-Propulsion System Simulation)
- **Subset:** FD001
- **Training engines:** 100
- **Test engines:** 100
- **Sensor measurements:** 21
- **Operating settings:** 3
- **Operating conditions:** 1
- **Fault mode:** HPC degradation

### Dataset Files

| File | Description |
|---|---|
| train_FD001.txt | Training engine operating and sensor data |
| test_FD001.txt | Test engine data with incomplete operating trajectories |
| RUL_FD001.txt | Actual remaining useful life at the final recorded cycle of each test engine |

The raw dataset is maintained locally and excluded from Git tracking.

## Technology Stack

- **Programming Language:** Python
- **Data Manipulation:** Pandas, NumPy
- **Development Environment:** Jupyter Notebook, VS Code, Anaconda
- **Version Control:** Git and GitHub

## Project Workflow

The project is organized into ten phases:

1. Project Setup and Data Understanding
2. Exploratory Data Analysis (EDA)
3. Feature Engineering
4. Data Preparation and Validation
5. Classification Models
6. Regression Models
7. Model Improvement and Hyperparameter Tuning
8. Model Explainability
9. Model Persistence and Deployment
10. Portfolio Documentation and GitHub

## Current Progress

**Phase 1 – Project Setup and Data Understanding**

Work completed so far:

- Loaded the FD001 training and test datasets.
- Assigned descriptive names to all 26 columns.
- Inspected dataset structure and dimensions.
- Identified unique engine IDs.
- Inspected operating cycles for individual engines.
- Loaded the test RUL file.
- Verified that the number of test engines matches the number of RUL records.
- Configured the local Git repository and connected it to GitHub.

## Planned Machine Learning Models

### Classification
- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier

### Regression
- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor

### Model Improvement and Explainability
- RandomizedSearchCV
- Feature selection
- SHAP explanations
- Model comparison and evaluation

## Planned Deployment

- Model persistence using Joblib
- Reusable prediction functions
- Streamlit application
- Engine health and Remaining Useful Life dashboard

## Repository Structure

```text
Intelligent-Predictive-Maintenance/
│
├── CMAPSSData/          # Local dataset (excluded from Git)
├── notes/
│   └── 01_Data_Understanding.ipynb
├── models/              # Saved models
├── results/             # Evaluation results
├── src/                 # Reusable Python modules
├── README.md
├── requirement.txt
├── .gitignore
└── LICENSE
```

## Project Status

Currently in development. The project will be updated progressively as each phase is completed, including EDA findings, feature engineering, model evaluation, and deployment.

## License

This project is licensed under the MIT License.
