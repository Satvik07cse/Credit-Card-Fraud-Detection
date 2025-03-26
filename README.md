# Credit Card Fraud Detection
## Overview
This project implements **Credit Card Fraud Detection** using **Anomaly Detection** techniques such as **Isolation Forest**, **Local Outlier Factor (LOF)**, and **One-Class SVM**. The dataset used contains real credit card transactions, with fraudulent cases being significantly rare.

## Dataset
- The dataset used is the **Credit Card Fraud Detection Dataset** from Kaggle.
- It consists of **284,807 transactions**, where **only 0.172% are fraudulent**.
- The features are **PCA-transformed** (except `Time` and `Amount`).
- The target column (`Class`) indicates whether a transaction is **fraudulent (1)** or **normal (0)**.

## Project Workflow
1. **Data Preprocessing**
   - Load the dataset and explore class distribution.
   - Perform **data visualization** (histograms, scatter plots, correlation heatmaps).
   - Sample **10%** of the data for efficient processing.
2. **Feature Engineering**
   - Separate independent (`X`) and dependent (`Y`) variables.
   - Normalize `Amount` for better performance.
3. **Anomaly Detection Models**
   - **Isolation Forest**: Tree-based method for detecting anomalies.
   - **Local Outlier Factor (LOF)**: Density-based anomaly detection.
   - **One-Class SVM**: Distance-based detection.
4. **Model Evaluation**
   - Train models and make fraud predictions.
   - Compute **accuracy, classification reports, and error rates**.
## Installation
To run this project, install the required dependencies:
```bash
pip install numpy pandas matplotlib seaborn scikit-learn
```
## Usage
Run the Python script:
```bash
python fraud_detection.py
```
## Results
- **Accuracy and Classification Reports** for all models are printed.
- **Fraud detection insights** are extracted from correlation analysis and time-based trends.

