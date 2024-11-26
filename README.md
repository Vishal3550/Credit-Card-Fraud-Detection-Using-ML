# Credit Card Fraud Detection Using Machine Learning

This repository contains a machine learning project designed to detect fraudulent credit card transactions. The system uses a logistic regression model and is deployed using a simple web application built with Streamlit.

## Project Overview

The goal of this project is to build a reliable fraud detection system that classifies credit card transactions as legitimate or fraudulent. This is achieved by:
1. Preprocessing the dataset to handle class imbalance using undersampling.
2. Training a logistic regression model on balanced data.
3. Deploying a user-friendly interface for fraud detection.

## Files in the Repository

1. **`Credit Card Fraud Detection using Machine Learning.ipynb`**
   - Jupyter Notebook that documents the entire process of data preprocessing, model training, evaluation, and visualization.

2. **`app.py`**
   - Python script to create a Streamlit-based web application for detecting fraud in real-time transactions.

3. **`creditcard.csv`**
   - The dataset used in the project. It contains anonymized features representing transaction details and a target class:
     - `0`: Legitimate transaction
     - `1`: Fraudulent transaction

## Features of the Application

- **Model Training:** 
   - Logistic regression model trained on a balanced dataset.
   - Metrics such as accuracy are calculated for both training and testing sets.

- **Web Application:**
   - Accepts feature values as input.
   - Predicts and displays whether a transaction is legitimate or fraudulent.

## Installation and Usage

### Prerequisites
- Python 3.7+
- Required libraries: 
  - `numpy`
  - `pandas`
  - `sklearn`
  - `streamlit`

### Steps to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/CreditCardFraudDetection.git
   cd CreditCardFraudDetection
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Launch the Streamlit application:
   ```bash
   streamlit run app.py
   ```

4. Enter the required feature values in the input fields and click "Submit" to see the prediction.

## Dataset Details

- **Source:** The dataset used in this project is anonymized and contains 31 columns, including:
  - Features `V1` to `V28`: Principal components obtained via PCA.
  - `Time` and `Amount`: Transaction timestamp and amount.
  - `Class`: Target variable indicating fraud (1) or legitimate (0).

## Model Summary

- **Algorithm:** Logistic Regression
- **Performance Metrics:**
  - Training Accuracy: ~calculated in app.py
  - Testing Accuracy: ~calculated in app.py

## Future Work

- Implement additional algorithms (e.g., Random Forest, XGBoost) for better performance.
- Explore techniques like SMOTE for balancing datasets.
- Enhance the web application with feature scaling and better input validation.
