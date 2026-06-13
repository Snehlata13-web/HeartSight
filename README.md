# HeartSight

A machine learning-powered web application for predicting heart disease risk using patient medical data.

## Overview

HeartSight uses a K-Nearest Neighbors (KNN) classifier trained on cardiovascular patient data to predict the likelihood of heart disease based on various medical parameters.

## Features

- Interactive web interface built with Streamlit
- Predicts heart disease risk based on:
  - Age
  - Sex
  - Chest pain type
  - Resting blood pressure
  - Cholesterol levels
  - Fasting blood sugar
  - Resting ECG results
  - Maximum heart rate
  - Exercise-induced angina
  - ST depression (Oldpeak)
  - ST slope

## Installation

```bash
pip install streamlit pandas joblib scikit-learn
```

## Usage

Run the application:

```bash
streamlit run app.py
```

## Project Structure

- `app.py` - Streamlit web application
- `HeartdiseaseFinal.ipynb` - Model training and EDA notebook
- `heart.csv` - Dataset with patient medical records
- `knn_heart_model.pkl` - Trained KNN model
- `heart_scaler.pkl` - Fitted StandardScaler for feature normalization
- `heart_columns.pkl` - Expected feature columns for model input

## Model

The classifier was trained using the K-Nearest Neighbors algorithm with standardized features. Multiple models were evaluated (Logistic Regression, Naive Bayes, Decision Tree, SVM) and KNN was selected based on accuracy and F1 score performance.