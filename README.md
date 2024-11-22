# Predictive-Analytics-for-Car-Prices
This project focuses on developing a machine-learning pipeline for predicting car prices. The dataset includes anonymized vehicle advertisements with attributes such as brand, type, mileage, and selling price. The task represents the challenges data science team faces in implementing price prediction models for online platforms.
The workflow includes data processing, feature engineering, model selection, hyperparameter tuning, and analysis

# Project Objectives 
Develop a regression model to predict car prices based on historical data.

Implement feature engineering and dimensionality reduction techniques to optimize the dataset.

Evaluate model performance using metrics like R-squared and Mean Absolute Error (MAE).

Provide insights into model interpretability through SHAP values and partial dependency plots.

# Dataset
The dataset includes approximately 400,000 rows with attributes such as:

Mileage, Model, Make, Price, Colour, Year of registration, Fuel type, Body type, Vehicle condition,  Reg_code.

# Methodology
1. Data Processing
Identified and addressed missing values, outliers, and erroneous entries (e.g., unrealistic registration years or zero mileage).

 Normalized numerical features and encoded categorical features using target encoding.

3. Feature Engineering
Derived new features like vehicle age from the year of registration.

 Introduced polynomial features (e.g., age², mileage²) and interaction terms to capture non-linear relationships.

3. Feature Selection
Performed manual and automated feature selection:

 Applied domain knowledge and automated methods (e.g., Recursive Feature Elimination with Cross-Validation) to identify the most predictive features.

 SelectKBest for identifying top predictors.

 Dimensionality reduction with PCA, though ultimately not used due to lower performance compared to polynomial regression.

4. Model Development
Built and evaluated multiple models:

 Linear Regression: Basic model for benchmarking.

 Random Forest: Captures non-linear relationships and interactions

 Gradient Boosting

 Ensemble Voting Regressor: Combined predictions from all models using a voting regressor for enhanced stability.

 Hyperparameter tuning using Grid Search.

5. Model Evaluation
Assessed performance using metrics such as:

 R-squared: Measures the proportion of variance explained.

 MAE: Evaluates average prediction error.

 True vs. Predicted plots and SHAP values provided insights into model accuracy and feature importance.

# Key Findings
Gradient Boosting emerged as the most accurate model with:

Test R-squared: 92%

MAE: 1572.19

Vehicle age, mileage, and model were identified as the most influential predictors.

Polynomial features significantly improved the predictive capability of linear models.

SHAP Analysis: Demonstrated the contribution of individual features to specific predictions, enhancing interpretability.

Partial Dependency Plots: Highlighted non-linear relationships, such as the impact of mileage and vehicle age on price depreciation.
