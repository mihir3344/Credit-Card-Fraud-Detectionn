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
| Model                        | Accuracy | Precision | Recall | F1 Score |
|------------------------------|----------|-----------|--------|----------|
| XGBoost                      | 0.9996   | 1.00      | 0.85   | 0.87     |
| LightGBM                     | 0.9992   | 0.70      | 0.87   | 0.77     |
| CatBoost                     | 0.9991   | 0.68      | 0.84   | 0.75     |
| Balanced Bagging Classifier  | 0.9991   | 0.69      | 0.74   | 0.71     |
| Logistic Regression          | 0.8916   | 0.01      | 0.96   | 0.03     |
| One-Class SVM                | 0.0006   | 0.00      | 0.40   | 0.00     |
| Random Forest                | 0.9996   | 0.95      | 0.77   | 0.85     |
| Decision Tree                | 0.9987   | 0.57      | 0.70   | 0.63     |

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
