# Credit-Card-Fraud-Detectionn
Credit Card Fraud Detection Project Overview
This project aims to detect fraudulent credit card transactions using machine learning techniques. The dataset consists of anonymized transaction data, with a class label indicating whether a transaction is fraudulent (1) or not (0). Due to the imbalanced nature of the data, techniques like SMOTE (Synthetic Minority Over-sampling Technique) are used to balance the dataset before model training.

Key Features

Transaction Amount: The amount of the transaction.
Time: Timestamp of the transaction.
Features: Anonymized features capturing transaction characteristics.
Class Label: 0 for non-fraudulent, 1 for fraudulent transactions.
Methodology

Data Preprocessing: Missing values are handled, features are engineered, and scaling is performed using RobustScaler.
Class Imbalance Handling: SMOTE generates synthetic data for fraudulent transactions.
Models Used:

XGBoost, LightGBM, CatBoost: Gradient boosting algorithms known for their high performance.
Balanced Bagging Classifier: Helps handle imbalanced datasets.
Logistic Regression & One-Class SVM: Baseline and outlier detection models.
Model Evaluation:
Models are evaluated on accuracy, precision, recall, and F1-score. Cross-validation and hyperparameter tuning are used for performance optimization.

Goal:
To identify the best-performing model for fraud detection, minimizing false negatives where fraud is missed.






