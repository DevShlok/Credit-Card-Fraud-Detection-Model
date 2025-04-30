# Credit Card Fraud Detection

This repository contains a machine learning project aimed at detecting fraudulent credit card transactions using supervised learning techniques. The model leverages a dataset of real-world credit card transactions, applying data preprocessing, feature engineering, and training a DecisionTreeClassifier for prediction.

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Model](#model)
- [Evaluation](#evaluation)
- [Results](#results)
- [Limitations & Future Work](#limitations--future-work)
- [License](#license)

---

## Project Overview

Credit card fraud is a critical problem in the financial industry. This project uses machine learning classification algorithms to identify potentially fraudulent transactions, helping financial institutions prevent losses.

## Dataset

- **Source:** [Kaggle Credit Card Fraud Detection Dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
- **Shape:** 284,807 transactions, 31 features.
- **Note:** Data is highly imbalanced, with <1% positive (fraudulent) cases.

## Features

- **V1 - V28:** Principal Components from PCA transformation (due to confidentiality).
- **Time:** Seconds elapsed between each transaction and the first.
- **Amount:** Transaction amount.
- **Class:** Target variable (0 = non-fraud, 1 = fraud).

## Installation

1. Clone the repository:
2. Install dependencies (Python 3.x required):
3. Download the dataset from [Kaggle](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud) and place it in the root directory.

## Usage

Open and run the Jupyter notebook:


Follow the notebook steps:
- Data loading
- EDA (Exploratory Data Analysis)
- Preprocessing (e.g., handling imbalance)
- Model training
- Model evaluation

## Model

- **Algorithm:** DecisionTreeClassifier (scikit-learn)
- **Preprocessing:** Handling missing data, class imbalance, feature selection.
- **Metrics:** Accuracy, precision, recall, F1-score, ROC AUC.

## Evaluation

The model was evaluated using standard metrics due to class imbalance:

================== Logistic Regression =================
Accuracy: 94.508 %
Precision: 97.322 %
Recall: 91.527 %
F1 Score: 94.336 %

================== Decision Tree Classifier =================
Accuracy: 99.825 %
Precision: 99.733 %
Recall: 99.918 %
F1 Score: 99.825 %

## Results

- The model successfully identifies fraudulent transactions with competitive recall and precision.
- Feature importance analysis is included.

## Limitations & Future Work

- **Imbalanced data:** Consider advanced sampling techniques like SMOTE or ensemble methods.
- **Model improvement:** Test additional algorithms (RandomForest, XGBoost, etc.).
- **Deployment:** Integrate with API for live prediction.



**Contributions welcome! Feel free to fork and improve this project.**

