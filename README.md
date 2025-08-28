# **Credit Card Fraud Detection**

📌 Project Overview

This project applies Python-based data analysis and machine learning to the problem of credit card fraud detection. Fraud detection is a critical issue in financial services, but it is made challenging by the extreme class imbalance (fraudulent transactions represent less than 0.2% of total data).

The analysis covers descriptive statistics, visualizations, and a Random Forest classifier to detect fraudulent transactions, emphasizing the importance of using precision, recall, and AUC metrics instead of raw accuracy
.

🔎 Dataset

Source: Kaggle – Credit Card Fraud Detection Dataset

Size: 284,807 transactions

Fraud Rate: 0.1727% (492 frauds, 284,315 non-frauds)

Features: 28 anonymized PCA components, Amount, and Time.

Target Variable: Class (0 = non-fraud, 1 = fraud).

🛠️ Methodology
1. Descriptive Analysis

Fraudulent transactions cluster in specific time windows.

Fraudulent transactions tend to have smaller monetary values compared to legitimate ones
.

2. Visualizations

Distribution of transaction amounts for fraud vs. non-fraud.

Time-based clustering of fraudulent activity.

Correlation heatmap of PCA-transformed features.

3. Advanced Analysis – Machine Learning

Model Used: Random Forest Classifier.

Key Metrics:

Precision = 0.9720

Recall = 0.7027

ROC-AUC = 0.9275

PR-AUC = 0.8152

📊 Key Findings

Accuracy is misleading in highly imbalanced datasets – precision, recall, and AUC provide a better evaluation framework.

Fraudulent patterns: Many frauds occur in rapid succession with low transaction amounts.

Random Forest Results: Balanced trade-off between high precision (few false positives) and good recall (detecting most frauds).

PCA-based Features: Even with anonymized PCA components, robust detection is possible, preserving privacy and interpretability.

📂 Deliverables

Assignment_A1.ipynb – Python notebook with preprocessing, analysis, visualization, and modeling code.

A1 Report.pdf – One-page summary report with findings and business implications
.

README.md – This documentation.

🚀 Business Implications

High Precision → Low disruption to legitimate users.

Good Recall → Reduced financial exposure by catching fraud early.

Scalability: Approach can be extended to real-time fraud monitoring.

Future Work:

Include live transaction streams.

Adapt models to evolving fraud tactics.

Integrate network-based fraud detection approaches
.

📜 References

Kaggle. (2018). Credit Card Fraud Detection Dataset. https://www.kaggle.com/mlg-ulb/creditcardfraud

Abi Joshua George. (2025). Assignment A1: Credit Card Fraud Detection Analysis Report. Hult International Business School
