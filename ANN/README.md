# Artificial Neural Network for Binary Classification (Fraud Detection)
## Project Overview
This project implements an Artificial Neural Network (ANN) to solve a binary classification problem using a real-world, highly imbalanced dataset. The objective is to accurately identify rare positive cases (fraud) while minimizing false positives.
The project demonstrates end-to-end machine learning workflow, including data preprocessing, feature scaling, model building, evaluation using advanced metrics, and performance tuning.

## Dataset
Source: Kaggle – Credit Card Fraud Detection
Description:
Transactions made by European cardholders.
Highly imbalanced dataset.
Target variable: Class.
0 → Normal transaction.
1 → Fraudulent transaction.

## Dataset link:
https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud

## Technologies Used
Python,
NumPy,
Pandas,
Scikit-learn,
TensorFlow / Keras,
Matplotlib.

## Data Preprocessing
The following preprocessing steps were applied:
Checked and handled missing (NaN) values.

## Feature scaling:
Converted data into NumPy arrays for ANN compatibility.
Split data into training and testing sets.
Ensured no data leakage during scaling.

## Model Architecture (ANN)
Input Layer: Based on number of features.
Hidden Layers:
Dense layers with ReLU activation.
Output Layer:
Sigmoid activation for binary classification.
Optimizer:
Adam.
Loss Function:
Binary Crossentropy.

## Model Evaluation Metrics
Since accuracy is misleading for imbalanced data, the following metrics were used:
ROC–AUC Score,
Precision,
Recall,
Precision–Recall Curve,
Validation Accuracy,
Validation metrics were automatically tracked using Keras during training.

## Performance Analysis
Used ROC–AUC to evaluate overall class separability.
Used Precision–Recall trade-off to analyze false positives vs false negatives.
Tuned decision threshold to improve recall for fraud detection.
Identified class imbalance issues and avoided relying solely on accuracy.

## Key Learnings
Neural Networks are highly sensitive to NaN values and feature scaling.
Accuracy alone is not a reliable metric for imbalanced datasets.
ROC–AUC and PR–AUC provide better performance insight.
Proper preprocessing significantly improves model stability.
