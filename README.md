Credit Card Fraud Detection Project
This project aims to detect fraudulent credit card transactions using machine learning models. The dataset contains anonymized transaction data, with a class label indicating whether a transaction is fraudulent (1) or not (0). Due to the imbalanced nature of the dataset, we use ADASYN (Adaptive Synthetic Sampling) to generate synthetic samples of fraudulent transactions before model training.

Key Features
Transaction Amount: The amount involved in each transaction.
Time: Timestamp of the transaction, indicating the sequence of transactions.
Features: Anonymized features that capture various characteristics of each transaction.
Class Label: Binary label where 0 = non-fraudulent and 1 = fraudulent.
Methodology
1. Data Preprocessing
Missing Values: Handled appropriately based on the type and amount of missing data.
Feature Engineering: Additional features are created if they improve model performance.
Scaling: Applied RobustScaler to manage the effect of outliers.
2. Handling Class Imbalance
ADASYN: Adaptive Synthetic Sampling generates synthetic data for the minority class (fraudulent transactions) to address dataset imbalance.
3. Models Used
XGBoost, LightGBM, CatBoost: Gradient boosting models known for high performance.
Balanced Bagging Classifier: Manages class imbalance by combining multiple weak classifiers.
Logistic Regression & One-Class SVM: Baseline models, including one specifically for outlier detection.
4. Model Evaluation
Each model is evaluated on accuracy, precision, recall, and F1-score.
Cross-validation and hyperparameter tuning are applied to optimize performance.
Project Goal
The primary goal is to identify the best-performing model for fraud detection, with a focus on minimizing false negatives (missed fraudulent transactions) while maintaining high accuracy.
| Model                   | Accuracy | Precision (Class 1) | Recall (Class 1) | F1-score (Class 1) |
|-------------------------|----------|----------------------|-------------------|---------------------|
| **XGBoost**             | 0.9994   | 0.76                | 0.88             | 0.81               |
| **LightGBM**            | 0.9989   | 0.61                | 0.83             | 0.71               |
| **CatBoost**            | 0.9991   | 0.66                | 0.88             | 0.75               |
| **Balanced Bagging**    | 0.9989   | 0.62                | 0.82             | 0.71               |
| **Logistic Regression** | 0.9884   | 0.11                | 0.90             | 0.20               |
| **One-Class SVM**       | 0.0012   | 0.00                | 0.77             | 0.00               |
| **Random Forest**       | 0.9995   | 0.82                | 0.88             | 0.85               |
| **Decision Tree**       | 0.9975   | 0.37                | 0.79             | 0.50               |

Conclusion
The Random Forest and XGBoost models perform the best for fraud detection, balancing accuracy, precision, and recall. Both effectively minimize false negatives, making them suitable for high-stakes fraud detection scenarios.

Simply copy and paste this markdown content into your README.md file on GitHub, and you’ll have a clean, professional overview ready to go!





