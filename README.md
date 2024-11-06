# Credit-Card-Fraud-Detectionn
Credit Card Fraud Detection
Project Overview
This project focuses on detecting fraudulent credit card transactions using machine learning techniques. It leverages several powerful classification algorithms including XGBoost, LightGBM, CatBoost, and others to predict fraudulent activities in credit card transactions. The dataset contains historical transaction data, and the model is designed to identify anomalies and potential fraud.

Dataset
The dataset used in this project consists of anonymized credit card transactions, where each transaction is labeled as either fraudulent or non-fraudulent. The data is imbalanced, with very few fraudulent transactions compared to the non-fraudulent ones, which poses a significant challenge. To address this, techniques like SMOTE (Synthetic Minority Over-sampling Technique) are used to balance the dataset before training the models.

Key Features:
Transaction amount: The amount of the transaction.
Time: Time of the transaction.
Features: Various anonymized features that capture transaction characteristics, which are used to detect fraudulent behavior.
Class label: Binary class indicating whether the transaction is fraudulent (1) or not (0).
Methodology
Data Preprocessing
Handling Missing Values: Missing data is cleaned or imputed.
Feature Engineering: Creating new features or transforming existing ones.
Class Imbalance Handling: Since fraudulent transactions are rare, we use SMOTE to generate synthetic samples for the minority class.
Scaling: Standard scaling techniques like RobustScaler are used to handle outliers and scale features.
Model Training
Multiple machine learning models are tested to predict fraudulent transactions:

XGBoost: A popular gradient boosting algorithm known for its high performance in classification tasks.
LightGBM: A gradient boosting framework that is efficient in terms of both speed and memory usage.
CatBoost: A gradient boosting model designed for categorical features but also performs well with continuous data.
Balanced Bagging Classifier: Uses ensemble methods to deal with imbalanced datasets.
Logistic Regression: A baseline model used for comparison.
One-Class SVM: A one-class classification algorithm that learns the distribution of the data and detects outliers.
Model Evaluation
Each model is evaluated based on its accuracy, precision, recall, and F1-score. The goal is to identify the model that performs best in detecting fraudulent transactions, especially minimizing false negatives, as missing fraudulent transactions is more costly than wrongly classifying a legitimate one as fraudulent.

Performance Optimization
Cross-validation: 5-fold cross-validation is used to assess the performance of each model.
Hyperparameter Tuning: Some models are tuned using grid search to find the best parameters.
Feature Selection: The most relevant features are selected to optimize the models’ performance.
