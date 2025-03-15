Project Overview

This project focuses on predicting employee attrition using various classification models. The dataset was preprocessed, balanced using under sampling due to class imbalance, and analyzed to identify key factors contributing to attrition. Multiple machine learning models were implemented and evaluated to determine the best-performing approach.

Dataset Description

The dataset includes numerical and categorical features related to employee demographics, job roles, and work conditions. The key preprocessing steps included:
Handling Missing Values: Filled in empty rows.
Feature Bifurcation: Separated categorical and numerical features.
Data Balancing: Applied undersampling due to class imbalance.
Outlier Treatment: Used IQR winsorization.
Encoding: One-Hot and Label Encoding for categorical variables.
Train-Test Split: Divided data into training (80%) and testing (20%).
Models Implemented & Performance

1. Logistic Regression
Training Accuracy: 63.21%
Training Precision: 64.18%
Testing Accuracy: 65.57%
Testing Precision: 67.88%
Observation: Baseline model, decent generalization but could be improved.

2. K-Nearest Neighbors (KNN)
Training Accuracy: 63.92%
Training Precision: 63.44%
Testing Accuracy: 48.48%
Testing Precision: 49.01%
Observation: Poor generalization, performs poorly on test data.

3. Support Vector Classifier (SVC)
Training Accuracy: 52.2%
Testing Accuracy: 51.29%
Observation: Poor performance, not suitable for this dataset.

4. Decision Tree Classifier
Training Accuracy: 100%
Testing Accuracy: 85%
Observation: Overfits training data but performs well on test data.

5. Random Forest Classifier
Training Accuracy: 99.79%
Testing Accuracy: 88.29%
Observation: Performs better than Decision Tree, with reduced overfitting.

6. XGBoost Classifier
Training Accuracy: 100%
Testing Accuracy: 90%
Observation: Best performer with high accuracy and better generalization.

7. Voting Classifier (Ensemble Model)
Training Accuracy: 100%
Testing Accuracy: 81%
Observation: Performs well but slightly lower than Random Forest and XGBoost.

Best Model Selection
Based on testing accuracy and generalization capability:
XGBoost Classifier performed the best with 90% testing accuracy, indicating it balances bias and variance well.
Random Forest Classifier also performed well with 88.29% accuracy and reduced overfitting.
Decision Tree, Voting Classifier, and KNN had lower performance due to either overfitting or underfitting.

Conclusion

XGBoost is the best model for this dataset. Random Forest is a strong alternative but slightly overfits.
