# 🤖 Classification using Logistic Regression and Naive Bayes
This project demonstrates **two classic classification algorithms** — **Logistic Regression** and **Naive Bayes** — applied on numerical and textual datasets respectively.

> 🚀 A great starting point for beginners in machine learning and natural language processing (NLP)!

## 🔍 Overview

### ✅ Logistic Regression:
- Performs binary classification on a small **numerical dataset**.
- Evaluates model using **accuracy score**.

### 🧠 Naive Bayes:
- Performs **text classification** (sentiment analysis) using the **bag-of-words** model.
- Evaluates using **accuracy**, **confusion matrix**, and **classification report**.

## 📦 Libraries Used
```python
# Logistic Regression
import numpy as np
from sklearn.model_selection import train_test_split
from sklearn.linear_model import LogisticRegression
from sklearn.metrics import accuracy_score

# Naive Bayes
import pandas as pd
from sklearn.feature_extraction.text import CountVectorizer
from sklearn.naive_bayes import MultinomialNB
from sklearn.metrics import classification_report, confusion_matrix

🧪 Part 1: Logistic Regression
🔢 Dataset:
A small sample numerical dataset defined using NumPy arrays.

🏗️ Steps:
1. Define features (x) and labels (y)
2. Split into training and testing sets
3. Train a LogisticRegression model
4. Predict test results
5. Evaluate using accuracy_score

🧠 Part 2: Naive Bayes for Text Classification
💬 Dataset:
Sample text reviews with binary sentiment labels (1 = positive, 0 = negative)

🏗️ Steps:
1. Create a pandas.DataFrame with text data
2. Split into training and testing sets
3. Use CountVectorizer to convert text into numerical format
4. Train a MultinomialNB classifier
5. Predict test results
6. Evaluate using:
  - Accuracy
  - Confusion Matrix
  - Classification Report

📊 Sample Output:
Logistic Regression Accuracy: 0.75
Naive Bayes Classification Report:
              precision    recall  f1-score   support
           0       0.80      1.00      0.89         4
           1       1.00      0.75      0.86         4

Confusion Matrix:
[[4 0]
 [1 3]]

🧠 What I Learned
- How to implement Logistic Regression for numeric data
- How to use Naive Bayes for text classification tasks
- How to preprocess and vectorize text using CountVectorizer
- How to evaluate classifiers using standard ML metrics

📜 License
This project is licensed under the MIT License – free to use, modify, and share.
