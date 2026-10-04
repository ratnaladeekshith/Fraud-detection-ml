# Credit Card Fraud Detection

## Project Overview

This project builds a machine learning model to detect fraudulent credit card transactions.

The project uses the ULB Credit Card Fraud Detection dataset and focuses on handling the severe class imbalance present in fraud detection.

## Dataset

The dataset contains 284,807 credit card transactions, including:

- 284,315 legitimate transactions
- 492 fraudulent transactions

Fraudulent transactions represent approximately 0.17% of the dataset.

## Machine Learning Approach

The project follows these steps:

1. Exploratory Data Analysis
2. Class imbalance analysis
3. Train-validation-test split
4. Feature scaling
5. Logistic Regression baseline
6. Random Forest classification
7. Decision threshold tuning
8. Final evaluation on unseen test data

## Models

### Logistic Regression

Used as the baseline machine learning model.

### Random Forest

Used as the final model because it performed better for the fraud detection task.

Class weighting was used to address the severe class imbalance.

## Evaluation

The model was evaluated using:

- Precision
- Recall
- F1-score
- Confusion Matrix

Because fraud transactions are highly imbalanced, accuracy alone was not considered sufficient.

## Final Result

The final Random Forest model achieved approximately:

- Fraud Precision: 83%
- Fraud Recall: 83%
- Fraud F1-score: 83%

On the test set, the model detected 81 out of 98 fraudulent transactions.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Project Structure

```text
fraud-detection-ml/
│
├── fraud_detection_analysis.ipynb
└── README.md
