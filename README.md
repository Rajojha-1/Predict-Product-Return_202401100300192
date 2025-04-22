#Raj Ojha 202401100300192
# Predict-Product-Return_202401100300192
# Predict Product Return

This project predicts whether a product will be returned based on purchase behavior data. It uses a machine learning model (Random Forest Classifier) trained on features like purchase amount, review score, and delivery time. The goal is to help e-commerce platforms reduce return rates and improve customer satisfaction.

## Model Overview

- Algorithm: Random Forest Classifier  
- Features:
  - purchase_amount
  - review_score
  - days_to_delivery
- Target: returned (yes/no)

## Dataset

The dataset includes historical transaction data with information about:
- Purchase amounts
- Review scores
- Delivery times
- Return status

File: `product_return.csv`  
Note: Ensure the dataset is cleaned (no missing values in key columns) and the `returned` column is binary encoded (`yes` = 1, `no` = 0).

## How It Works

1. Load and preprocess the data
2. Train-test split (80/20)
3. Apply hyperparameter tuning with GridSearchCV
4. Train the best Random Forest model
5. Take user input for prediction
6. Show visual insights:
   - Purchase distribution
   - Review scores vs. return status
   - Delivery days analysis
   - Confusion matrix and performance metrics

## Visualizations

The notebook generates the following plots:
- Purchase Amount Distribution by Return Status
- Review Score vs Return Status (Boxplot)
- Delivery Days vs Return Status (Violinplot)
- Confusion Matrix (Heatmap)

## Evaluation Metrics

- Accuracy Score
- Classification Report (Precision, Recall, F1-score)
- Confusion Matrix

## Requirements

- Python 3.7+
- pandas
- matplotlib
- seaborn
- scikit-learn
