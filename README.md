# Credit Card Fraud Data Analysis Project

**Important:** This credit card fraud dataset is an imbalanced dataset.

## Introduction

This project aims to analyze credit card fraud data using various machine learning algorithms. The dataset contains transactions labeled as fraudulent or non-fraudulent, and the goal is to build classification models to accurately identify fraudulent transactions. The analysis includes preprocessing steps, classification model training, evaluation of model performance metrics, and comparison of computational efficiency.

## Setup

To replicate the project, follow these steps:

1. Install necessary libraries using `pip install kaggle` and `pip install lightgbm`.
2. Set up Kaggle API credentials for downloading the dataset.
3. Download the credit card fraud dataset using Kaggle API.
4. Unzip the downloaded dataset.

## Data Preprocessing

The dataset is preprocessed to handle missing values and normalize the data for better model performance. Additionally, sampling techniques are applied to address the class imbalance issue between fraudulent and non-fraudulent transactions.

## Model Training and Evaluation

Various classification algorithms such as Decision Tree, Random Forest, XGBoost, AdaBoost, Gradient Boost, and LightGBM are trained on the preprocessed data. Model performance is evaluated using metrics like F1 score, accuracy, precision, recall, and computational efficiency measured in fit runtime.

## Results and Discussion

### Model Accuracy Metric

Based on F1 score, the ranking of models is as follows:
1. XG Boost: 0.921
2. Gradient Boosting: 0.922
3. Random Forest: 0.923
4. Ada Boost: 0.914
5. LGBM: 0.920
6. Decision Tree: 0.892

### Computational Performance Metric

Ranked by fit runtime:
1. Decision Tree: 0.026 seconds
2. XG Boost: 0.297 seconds
3. Ada Boost: 0.317 seconds
4. LGBM: 0.472 seconds
5. Random Forest: 0.488 seconds
6. Gradient Boost: 1.089 seconds

### Normalized vs Not Normalized

Normalization improves runtime speed by approximately 31.44% across all algorithms.

### Effect of Sampling

Sampling techniques significantly impact model accuracy, emphasizing its importance in addressing class imbalance.

## Conclusion

In conclusion, XG Boost and Gradient Boosting demonstrate the highest F1 scores, indicating strong model accuracy. However, Decision Tree stands out for its superior computational efficiency. Normalization enhances runtime speed, while sampling techniques play a crucial role in improving model accuracy. These findings underscore the importance of selecting appropriate algorithms and preprocessing techniques to achieve optimal performance in fraud detection tasks.
