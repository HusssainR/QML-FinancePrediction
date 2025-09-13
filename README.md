# Quantum-Inspired Finance Classifier

This project explores **quantum-inspired machine learning techniques** for financial risk classification.  
It combines **classical financial feature engineering** with **quantum kernel methods** to assess portfolio risk and evaluate the performance of **quantum-enhanced classifiers** compared to standard SVM baselines.  

---

## Overview

Traditional finance models rely on statistical measures like volatility or Sharpe ratios.  
This project extends those methods by:

1. **Data Acquisition** – Using `yfinance` to fetch historical stock price data across major U.S. sectors.  
2. **Feature Engineering** – Extracting volatility, Sharpe ratio, and maximum drawdown to represent portfolio risk.  
3. **Risk Labeling** – Categorizing assets into **low**, **medium**, or **high** risk based on thresholds.  
4. **Classical Baseline** – Training a classical **SVM classifier** on extracted features.  
5. **Quantum Extension** – Applying **Qiskit’s ZZFeatureMap** and **QuantumKernel** to construct a quantum kernel SVM (QSVC).  
6. **Visualization** – Generating plots (pair plots, scatter analyses, boxplots) to analyze distributions and feature separability.  

This pipeline demonstrates how **quantum feature maps** can potentially capture nonlinear structures in financial data, offering insights for **quantum finance** applications.

---

## Features

- End-to-end ML pipeline for financial risk classification  
- Custom risk labeling system using volatility, Sharpe ratio, and drawdown  
- Baseline **SVM classifier** with performance reports  
- **Quantum kernel SVM** (QSVC) using `Qiskit Machine Learning`  
- Automated **data visualization** (pairplots, scatter plots, boxplots) for interpretability  
- Exportable dataset (`labeled_features.csv`)  

---

## Tech Stack

- **Python 3.9+**
- [pandas](https://pandas.pydata.org/) – data wrangling  
- [numpy](https://numpy.org/) – numerical computations  
- [yfinance](https://pypi.org/project/yfinance/) – financial data acquisition  
- [scikit-learn](https://scikit-learn.org/) – classical ML pipeline (SVM, PCA, train/test splits)  
- [matplotlib](https://matplotlib.org/) & [seaborn](https://seaborn.pydata.org/) – plotting  
- [Qiskit](https://qiskit.org/) – quantum kernel methods  

---

## Example Results  

### Classical SVM Baseline  
- Accuracy: ~88% on test set  
- Strong performance on medium-risk assets  

### Quantum Kernel SVM  
- Comparable performance to classical baseline  
- Shows potential for improved **nonlinear separability** in financial data  

---

## Dataset  
- **Assets**: 100+ U.S. equities across 11 sectors (Technology, Energy, Financials, etc.)  
- **Timeframe**: 2020–2025  
- **Risk classes**:  
  - **Low** – stable returns, low volatility  
  - **Medium** – balanced risk/reward  
  - **High** – volatile, low Sharpe ratio  

---

## Future Work  
- Extend feature set (e.g., beta, skewness, sector correlations)  
- Deploy on **IBM Quantum hardware** for small-scale experiments  
- Explore **quantum variational classifiers** beyond kernel methods  
- Benchmark against **deep learning models** for risk prediction  

