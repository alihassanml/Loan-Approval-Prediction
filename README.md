# Loan Approval Prediction

This project focuses on predicting loan approval using machine learning algorithms. The model takes various customer features as input and predicts whether a loan application will be approved or not. Key steps in the workflow include data preprocessing, feature engineering, model selection, and hyperparameter tuning.

## Project Overview

- **Dataset:** Includes features related to loan applicants such as income, credit history, loan amount, etc.
- **Objective:** Build a model to predict loan approval status.
- **Methods Used:** Decision Trees, GridSearchCV for hyperparameter tuning, and PCA for dimensionality reduction.

## Key Features

1. **Data Preprocessing:** 
    - Handle missing values, scaling, and encoding categorical features.
  
2. **Modeling:**
    - Use Decision Tree Classifier as the base model.
    - Perform hyperparameter tuning with GridSearchCV to optimize model performance.

3. **Evaluation Metrics:**
    - Accuracy Score: `0.96`
    - Confusion Matrix and Classification Report show excellent performance on precision, recall, and F1-score.

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/alihassanml/Loan-Approval-Prediction.git
    ```
2. Install the necessary dependencies:
    ```bash
    pip install -r requirements.txt
    ```

## Usage

1. Open the Jupyter Notebook:
    ```bash
    jupyter notebook Loan_Approval_Prediction.ipynb
    ```

2. Follow the steps in the notebook to preprocess data, build, and evaluate the model.

## Hyperparameter Tuning

- **Parameters Tuned:** 
    - Criterion: ['gini', 'entropy', 'log_loss']
    - Splitter: ['best', 'random']
    - Max Depth: [1, 5, 10, 15, 20, 25, 30]
    - Max Features: ['auto', 'sqrt', 'log2']

- Best parameters were selected using 5-fold cross-validation for optimal accuracy.

## Results

- **Accuracy Score:** `0.96`
- **Confusion Matrix:**
    ```
    [[854  33]
     [ 23 499]]
    ```
- **Classification Report:**
    ```
                  precision    recall  f1-score   support
           0       0.97      0.96      0.97       887
           1       0.94      0.96      0.95       522
    ```

## Future Work

- Explore other classification algorithms like Random Forest, SVM, or XGBoost.
- Further optimize the model with additional feature engineering techniques.
