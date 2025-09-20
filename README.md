# 🌲 Forest Cover Classification

## 📌 Overview

This project aims to classify different **types of forest cover** based on environmental and geographical attributes. The dataset is **highly imbalanced**, with the majority of samples in classes 1 and 2, while classes 4–7 have very few examples. To address this, the project explores **class balancing techniques** such as weighted classifiers and XGBoost’s `scale_pos_weight`.

## 🛠️ Workflow

1. **Data Exploration & Preprocessing**

   * Checked for missing values and feature distributions.
   * Scaled/normalized features where necessary.
   * Split dataset into training and testing sets.

2. **Model Training**

   * Implemented Logistic Regression, Random Forest, and XGBoost.
   * Applied **class weighting** and imbalance handling strategies.
   * Compared baseline vs. balanced models.

3. **Evaluation**

   * Accuracy, Precision, Recall, and F1-score (per class).
   * Confusion matrices with seaborn heatmaps for visualization.
   * Feature importance analysis for tree-based models.

## 📊 Results & Insights

* Standard models favored majority classes, leading to poor performance on minority classes.
* Using **class weights** and **scale\_pos\_weight** improved fairness across all categories.
* XGBoost and Random Forest performed best overall, with XGBoost showing strong handling of imbalance when tuned properly.

## 🚀 Future Work

* Hyperparameter tuning for improved generalization.
* Advanced resampling (SMOTE, ADASYN, undersampling).
* Testing deep learning models (ANN, CNN) for higher accuracy.

## 💻 Tech Stack

* Python, pandas, numpy
* scikit-learn, xgboost, imbalanced-learn
* seaborn, matplotlib

