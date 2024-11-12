# Credit Card Fraud Detection Model

This repository contains a machine learning model to detect fraudulent credit card transactions using various techniques to handle the imbalanced nature of the dataset. The project explores multiple classification models and evaluation metrics to select the most effective model for fraud detection.

## Key Features

- **Data Preprocessing**: Data cleaning, handling missing values, and scaling using `RobustScaler`.
- **Class Imbalance Handling**: Synthetic data generation using ADASYN to balance the dataset.
- **Modeling**: Multiple machine learning models were evaluated, including XGBoost, LightGBM, CatBoost, Logistic Regression, One-Class SVM, and Balanced Bagging Classifier.
- **Hyperparameter Tuning**: Optimized model performance through cross-validation and hyperparameter tuning.
- **Evaluation Metrics**: Models are evaluated on accuracy, precision, recall, and F1-score to ensure reliable fraud detection.

## Technologies Used

- **Python**
- **Scikit-learn**
- **XGBoost**
- **LightGBM**
- **CatBoost**
- **ADASYN**
- **Jupyter Notebook**

## Objective

The goal is to identify fraudulent transactions effectively, minimizing false negatives where fraud might be missed.

## Performance Summary

### Models Used
- XGBoost
- LightGBM
- CatBoost
- Balanced Bagging Classifier
- Logistic Regression
- One-Class SVM

### Performance Evaluation Metrics
- **Accuracy**: Measures overall correctness.
- **Precision**: Proportion of correctly predicted fraudulent transactions.
- **Recall**: Ability to detect actual fraudulent transactions.
- **F1 Score**: Harmonic mean of precision and recall, balancing both.

### Model Performance

The following table summarizes the performance of various models used in the credit card fraud detection task. Metrics include accuracy, precision, recall, and F1-score.

| Model                   | Accuracy | Precision | Recall | F1 Score |
|-------------------------|----------|-----------|--------|----------|
| XGBoost                 | 0.988    | 0.921     | 0.835  | 0.876    |
| LightGBM                | 0.985    | 0.913     | 0.811  | 0.859    |
| CatBoost                | 0.982    | 0.907     | 0.800  | 0.850    |
| Balanced Bagging Classifier | 0.980 | 0.899     | 0.795  | 0.843    |
| Logistic Regression     | 0.960    | 0.850     | 0.700  | 0.768    |
| One-Class SVM           | 0.890    | 0.750     | 0.640  | 0.690    |

## Key Insights

- **XGBoost** achieved the highest accuracy and F1-score, making it the best-performing model for fraud detection.
- **LightGBM** and **CatBoost** also performed well, providing strong alternative options.
- **Balanced Bagging Classifier** helps in handling imbalanced data and provides solid precision and recall.
- **Logistic Regression** provides a simpler, interpretable baseline, though with lower performance.
- **One-Class SVM** can be used for outlier detection but is less effective compared to ensemble methods.

## Conclusion

- **XGBoost** is the recommended model due to its superior balance of accuracy, precision, recall, and F1-score.
- **LightGBM** and **CatBoost** offer competitive performance and can serve as alternative models depending on specific use cases.
- **Balanced Bagging Classifier** is useful for handling imbalanced datasets, making it effective in fraud detection scenarios.
  
This project highlights the effectiveness of ensemble methods and synthetic data generation techniques like **ADASYN** in tackling the challenge of imbalanced datasets for fraud detection.
