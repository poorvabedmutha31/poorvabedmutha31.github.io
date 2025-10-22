---
layout: page
title: Exercise Prediction System
description: Predicting daily exercise habits using machine learning
img: assets/img/4.jpg
importance: 3
category: work
github: https://github.com/poorvabedmutha31/Do-you-exercise-
---

## Project summary
This exploratory health analytics project predicts whether a person exercises daily using self-reported lifestyle and vitals. It served as an early sandbox for building interpretable classification models that could later inform wellbeing recommendation systems.

## Approach
- Cleaned and imputed a Kaggle medical lifestyle dataset, engineering features such as BMI buckets, stress level encodings, and physician visit frequency.
- Trained logistic regression, gradient boosting, and random forest models with stratified cross-validation while tackling severe class imbalance via SMOTE.
- Generated SHAP explanations and counterfactual recourses so that end users could understand how incremental habit changes affect the prediction.

## Outcomes
- Achieved 89% accuracy and a Matthews correlation coefficient of 0.62 on the held-out set while maintaining calibrated probabilities.
- Produced clinician-facing dashboards that highlight top contributing features and provide “next best action” suggestions.
- Shared the pipeline with the UCSD Health recommendation team to guide features feeding into our production experimentation framework.

## Tools
- Python, pandas, scikit-learn, imbalanced-learn, SHAP, Plotly Dash.
- Deployed via Docker for reproducible experimentation and collaboration with public health teammates.

**[View on GitHub](https://github.com/poorvabedmutha31/Do-you-exercise-){:target="_blank"}**
