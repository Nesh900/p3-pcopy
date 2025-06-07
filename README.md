# Stroke Prediction Using Machine Learning

This repository contains a machine learning project aimed at predicting the risk of stroke in individuals using health-related data. The analysis includes data cleaning, exploratory data analysis (EDA), model development, and performance evaluation.

## Project Objectives

- Perform exploratory data analysis (EDA) to identify key factors associated with stroke.
- Develop a baseline classification model to benchmark performance.
- Build and tune machine learning models to predict stroke risk.
- Evaluate models using metrics such as accuracy, recall, precision, and F1-score.
- Provide business recommendations based on insights from the analysis.

## Dataset

The dataset used is publicly available and contains medical and demographic features including:
- Age
- Hypertension
- Heart Disease
- Work Type
- Smoking Status
- BMI
- Glucose Level
- Stroke Occurrence (target)

## Exploratory Data Analysis (EDA)

EDA was conducted to uncover patterns, correlations, and outliers in the data:
- Distribution of stroke across age, gender, and health conditions
- Correlation between features
- Class imbalance analysis
- Visualizations include bar plots, histograms, and correlation heatmaps

## Modeling and Evaluation

Several models were evaluated including:
- Logistic Regression (with and without SMOTE)
- Random Forest Classifier
- Hyperparameter tuning using GridSearchCV
- Performance metrics: Accuracy, Recall, Precision, F1 Score, ROC-AUC

### Best Performing Model
- **Logistic Regression (SMOTE + Tuning)**
- **Recall (stroke):** 0.84
- **Precision (stroke):** 0.12
- **F1-score (stroke):** 0.22

### Note
Recall was prioritized over precision to reduce false negatives in stroke detection.

## Key Results

- Significant class imbalance addressed using SMOTE.
- High recall in stroke prediction shows potential for early risk flagging.
- False positives were increased, indicating a tradeoff for higher sensitivity.

## Business Recommendations

- Use the model to flag at-risk individuals for further medical screening.
- Collect additional features (e.g., cholesterol, physical activity) to enhance model accuracy.
- Monitor and regularly update the model with new data to improve performance.

## Next Steps

- Feature engineering (interaction terms, polynomial features).
- Implement cost-sensitive learning.
- Integrate SHAP for model interpretability.
- Consider deploying the model via a simple web app.


