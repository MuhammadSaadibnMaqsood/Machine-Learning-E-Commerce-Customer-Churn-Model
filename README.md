# E-Commerce Customer Churn Prediction

## Problem Statement
E-commerce businesses need to identify customers who are likely to stop purchasing so they can take proactive retention actions. This project uses customer behavior and engagement data to build a machine learning model that predicts whether a customer is likely to churn.

## What This Project Does
The notebook in this repository loads customer feature and target datasets, prepares the data for modeling, explores the data distribution, trains a Logistic Regression model, and evaluates its performance using accuracy, classification metrics, and a confusion matrix.

## Data Used
- ecommerce_customer_features.csv
  - Customer features such as account age, order value, order frequency, purchase recency, discounts, returns, support interactions, browsing activity, cart abandonment, review scores, engagement, satisfaction, and price sensitivity.
- ecommerce_customer_targets.csv
  - Target labels for customer churn status.

## Workflow in the Notebook
1. Load the CSV files and remove the Customer_ID column from the modeling data.
2. Encode categorical variables using LabelEncoder so the model can process them.
3. Check for missing values in the datasets.
4. Split the data into training and testing sets.
5. Standardize numerical features for model stability.
6. Visualize data distributions with histograms and density plots.
7. Apply QuantileTransformer to selected numeric features to improve feature scaling behavior.
8. Train a Logistic Regression model on the training set.
9. Evaluate the model on the test set using:
   - Accuracy score
   - Classification report
   - Confusion matrix heatmap

## Solution Approach
The solution uses a supervised learning pipeline for binary classification:
- Input: customer behavior and engagement features
- Output: predicted churn class
- Model: Logistic Regression

This approach provides a simple and interpretable baseline for churn prediction, which is useful for understanding customer risk and supporting retention strategies.

## Expected Outcome
The model helps identify high-risk customers and provides measurable performance indicators to decide whether the baseline solution is suitable for deployment or needs further improvement.

## How to Run
Open the notebook and execute the cells in order.
