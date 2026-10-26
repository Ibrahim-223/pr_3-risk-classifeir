# Credit Risk Classification – Conceptual Understanding

## Overview

This section covers the basic concepts of classification, performance metrics, classification errors, and imbalanced data in machine learning.

## 1. What is Logistic Regression?

Logistic Regression is a machine learning algorithm used for classification. It predicts the probability of a class, such as whether a customer is high-risk or low-risk.

It is suitable for binary classification problems.

## 2. Classification Performance Metrics

Performance metrics help us evaluate how well a classification model performs.

- **Accuracy:** Percentage of correct predictions.
- **Precision:** How many predicted positive cases are actually positive.
- **Recall:** How many actual positive cases are correctly identified.
- **F1-Score:** Balance between precision and recall.

Accuracy alone is insufficient for imbalanced datasets because a model can achieve high accuracy while missing many minority-class cases.

## 3. Type-I Error and Type-II Error

In risk prediction:

- **Type-I Error (False Positive):** A low-risk customer is incorrectly predicted as high-risk.
- **Type-II Error (False Negative):** A high-risk customer is incorrectly predicted as low-risk.

False negatives can be costly because risky customers may not be identified.

## 4. Precision, Recall, F1-Score, TPR, and FPR

- **Precision:** The proportion of predicted high-risk customers who are actually high-risk.
- **Recall:** The proportion of actual high-risk customers correctly identified.
- **F1-Score:** The harmonic mean of precision and recall.
- **TPR (True Positive Rate):** The proportion of actual positive cases correctly identified. It is equal to recall.
- **FPR (False Positive Rate):** The proportion of actual negative cases incorrectly predicted as positive.

## 5. What is AUC-ROC?

ROC (Receiver Operating Characteristic) is a curve that shows the relationship between True Positive Rate and False Positive Rate at different classification thresholds.

AUC (Area Under the Curve) measures how well a model distinguishes between two classes. A higher AUC generally indicates better class separation.

## 6. Problems with Imbalanced Data

Imbalanced data occurs when one class has many more examples than another.

For example, if most customers are low-risk and only a few are high-risk, a model may favor low-risk predictions. This can lead to poor detection of high-risk customers even when accuracy is high.

## Conclusion

Classification models should be evaluated using multiple performance metrics rather than accuracy alone. For credit risk prediction, recall, F1-score, and false negatives are especially important because identifying high-risk customers can help reduce financial losses.
