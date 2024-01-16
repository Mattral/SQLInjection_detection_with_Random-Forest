# SQL Injection Detection System

## Overview

Simple demo project. This project implements a real-time SQL injection detection system using machine learning. A trained machine learning model will predicts whether an SQL query is safe or potentially malicious.

## Setup

1. Install dependencies:
    ```bash
    pip install flask scikit-learn requests joblib pandas
    ```

2. Train the model:
    ```bash
    python model.py
    ```

3. Run the Flask app:
    ```bash
    python app.py
    ```

4. Test predictions:
    ```bash
    python tester.py
    ```

## Files

- `sql_injection_model.pkl`: Trained machine learning model.
- `tfidf_vectorizer.pkl`: TF-IDF vectorizer used for text preprocessing.

## Usage

- The Flask app is accessible at `http://127.0.0.1:5000/`.
- Send POST requests to `http://127.0.0.1:5000/predict` with JSON data containing the SQL query for real-time predictions.

## Important Note

This project is a simplified example, and additional considerations such as security, scalability, and error handling should be addressed for production use.
