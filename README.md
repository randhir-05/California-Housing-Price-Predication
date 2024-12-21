# California-Housing-Price-Predication
<img width="916" height="400" alt="Screenshot 2024-12-21 at 8 36 12 PM" src="https://github.com/user-attachments/assets/cf76cf64-688b-4cc7-9cdf-7ff513c95a25" />

  # Project Summary
# Dataset Overview

Source: California Housing Prices dataset from the book Hands-On Machine Learning with Scikit-Learn and TensorFlow by Aurélien Géron.

Features: 10 variables, including:

longitude and latitude – geographical location.

housing_median_age – median age of houses.

total_rooms, total_bedrooms, population, households – housing-related metrics.

median_income – income metric.

median_house_value – target variable.

ocean_proximity – categorical variable.

# Objective

To build a predictive model for median_house_value using machine learning techniques and provide actionable insights through exploratory data analysis and feature engineering.

# Methodology

# 1. Data Preprocessing

Handling Missing Values:

Imputed missing values in total_bedrooms using the median strategy.

Feature Engineering:

Created new features: rooms_per_household, bedrooms_per_room, population_per_household.

Addressing Skewness:

Applied log transformations on right-tailed distributions.

# 2. Exploratory Data Analysis (EDA)

Visualizations:

Pair plots and histograms to understand feature distributions.

Correlation heatmaps to identify multicollinearity.

Scatter plots to examine geographical trends.

Insights:

Features like median_income show strong correlation with the target variable.

Multicollinearity addressed by feature selection.

# 3. Model Building and Evaluation

Models Evaluated:

Linear Regression

Random Forest Regressor

Support Vector Machines (SVM)

XGBoost Regressor

Metrics Used:

Root Mean Square Error (RMSE)

Mean Absolute Percentage Error (MAPE)

R² score

Hyperparameter Tuning:

Used GridSearchCV to fine-tune XGBoost parameters.

# 4. Final Model Selection

Best Model: XGBoost Regressor

RMSE: ~46,000

R² Score: 0.80

MAPE: ~17%

Reason for Selection:

Best overall performance across metrics.

Robust against overfitting as validated through cross-validation.

# 5. Deployment-Ready Model

Saved the model using pickle for easy deployment.

Key Findings

Median income is the most significant predictor of housing prices.

Geographical trends show higher prices near the ocean and urban areas.

Random Forest and XGBoost outperform simpler models like Linear Regression.

# Results and Outcomes

Prediction Accuracy: RMSE of ~46,000 and R² score of 0.82.

Insights:

Significant variables influencing housing prices.

Addressed data challenges like missing values and multicollinearity.

Deliverables:

A deployable XGBoost model.

Comprehensive visualizations and analysis.

