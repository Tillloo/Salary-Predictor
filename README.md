# Income Classification & Dataset Fairness Analysis


https://github.com/user-attachments/assets/adb3b4ca-485f-4dde-b463-877620a54f8a


# Check out the app here: https://salary-predictor-new.vercel.app/

# Overview

This project explores how different datasets affect the performance and fairness of income classification models. We compare two socioeconomic datasets using identical preprocessing and modeling pipelines to isolate the impact of dataset composition on predictions and bias.

We train XGBoost classifiers on each dataset and analyze differences in accuracy, feature importance, and fairness across demographic groups.

# Key Idea

Even with the same model and training process, dataset choice alone can significantly change both predictions and fairness outcomes.

# Datasets
UCI Adult Dataset
ACS Census Dataset

Both datasets were cleaned, standardized, and aligned to a shared feature space for fair comparison.

# Method
Identical preprocessing pipeline for both datasets
XGBoost classifier used for both models
Grid search hyperparameter tuning
Evaluation using accuracy, F1, ROC-AUC
Fairness analysis across gender and race

# Results

UCI Adult Dataset:

Accuracy: 87.8%
ROC-AUC: 0.93

ACS Dataset:

Accuracy: 71.2%
ROC-AUC: 0.84

# Key Findings
UCI dataset performs better but is less complex
ACS dataset shows more variability and lower accuracy
Both datasets exhibit measurable demographic disparities
Bias patterns are largely inherited from the data itself

# Fairness Analysis

We evaluate fairness using:

Demographic Parity
True Positive Rate (Equal Opportunity)
False Positive Rate

Consistent gaps are observed across gender and race groups.

# Interactive Frontend

A React-based web application was developed to support this analysis. It allows users to:

Input demographic and socioeconomic features
Generate real-time income predictions
Explore how predictions vary across groups
Interactively observe fairness-related differences

# Conclusion

This project shows that dataset choice alone can significantly impact both model performance and fairness, highlighting the importance of data-centric evaluation in machine learning systems.
