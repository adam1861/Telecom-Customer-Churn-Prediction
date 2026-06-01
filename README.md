# Telecom Customer Churn Prediction

Machine learning project for predicting telecom customer churn using exploratory data analysis, preprocessing, feature encoding, and classification models.

## Overview

This project analyzes customer data from a telecom churn dataset to identify patterns that are associated with customer attrition. The workflow covers data cleaning, categorical encoding, train/test splitting, model training, and evaluation.

## Project Workflow

1. Load the raw dataset.
2. Check and clean missing values and whitespace-only entries.
3. Convert selected Yes/No columns into binary values.
4. One-hot encode categorical features.
5. Convert `TotalCharges` to a numeric type.
6. Split the dataset into training and testing sets.
7. Train and evaluate machine learning models.

## Models Used

- Linear Regression
- Logistic Regression

For classification, Logistic Regression is the more appropriate model for churn prediction.

## Evaluation Metrics

The models are evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix

## Repository Structure

- `Notebooks/EDA.ipynb` - data cleaning, feature engineering, and dataset splitting
- `Notebooks/ML.ipynb` - model training and evaluation
- `raw_data/` - original dataset files
- `ready_data/` - exported train/test CSV files

## Dataset Preparation Notes

- `Partner`, `Dependents`, `PhoneService`, `PaperlessBilling`, and `Churn` are converted from Yes/No to binary values.
- `gender` is mapped to numeric values.
- Categorical columns are one-hot encoded.
- `customerID` is removed after a mapping copy is kept for reference.
- `TotalCharges` is converted to numeric.

## Getting Started

Open the notebooks in VS Code or Jupyter and run them in order:

1. `Notebooks/EDA.ipynb`
2. `Notebooks/ML.ipynb`

If the train/test CSV files are not present, run the export cell in the EDA notebook first.

## Result

The project shows that Logistic Regression performs better than the baseline linear approach for churn classification.
