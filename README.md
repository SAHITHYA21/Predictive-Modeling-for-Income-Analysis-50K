# Predictive Modeling for Income Analysis 50K

This project analyzes the Census Income dataset to predict whether individuals earn over USD 50,000 per year. It demonstrates data cleaning, preprocessing, exploratory data analysis (EDA), and the application of various machine learning models for binary classification.

## Overview
The objective is to apply machine learning techniques to classify individuals based on their income level. The project achieves a high level of accuracy (86.67%) using the Gradient Boosting Classifier and provides insights into income distribution patterns.

## Dataset
The dataset used is the [Adult Census Income Dataset](https://doi.org/10.24432/C5XW20) from the UCI Machine Learning Repository. It contains information about demographic and employment attributes.

## Features
- **Age**
- **Workclass**
- **Education**
- **Occupation**
- **Race**
- **Gender**
- **Hours per week**
- ...and more.

The target variable is income, categorized as `<=50K` or `>50K`.

## Key Steps
### 1. Data Cleaning
- Removed 24 duplicate rows to maintain data integrity.
- Handled missing values:
  - Replaced `?` with `NaN`.
  - Imputed missing entries in `workclass` and `occupation` using the mode.
  - Categorized missing values in `native-country` as "Unknown."
- Converted float columns to integers for consistency.
- Encoded categorical variables using `LabelEncoder`.

### 2. Exploratory Data Analysis (EDA)
- **Income vs. Gender:** Males have a higher proportion in the higher income bracket.
- **Income Distribution by Education Level:** Higher education levels are positively correlated with higher income.
- **Workclass Distribution:** Most individuals work in the private sector.

### 3. Machine Learning Models
- **Support Vector Machine (SVM)**
- **Gradient Boosting Classifier**
- **Decision Tree**
- **Random Forest**

Each model was trained and evaluated using accuracy scores and confusion matrices. The Gradient Boosting Classifier achieved the best performance with an accuracy of 86.67%.

### 4. Model Evaluation
- Accuracy Score: Measures the proportion of correct predictions.
- Confusion Matrix: Provides a breakdown of correct and incorrect predictions for each class.

## Results
- Achieved an overall accuracy of **86.67%** using the Gradient Boosting Classifier.
- Identified key insights into income inequality based on demographic and employment factors.

## Tools and Libraries
- **Python**
- **scikit-learn**: For model implementation.
- **pandas**: For data manipulation.
- **matplotlib** and **seaborn**: For visualizations.

## Getting Started
### Prerequisites
- Python 3.7+
- Libraries: `pandas`, `numpy`, `scikit-learn`, `matplotlib`, `seaborn`

