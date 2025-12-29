# House-Price-Prediction-Using-Multiple-Machine-Learning-Regression-Models

This project focuses on **building, training, and comparing multiple regression models** to predict **house price per unit area**.  
The goal is to identify the model that provides the **best balance of accuracy, interpretability, and performance** for the given dataset.

# Overview
Predicting house prices is a classic **regression problem** in machine learning.  
In this project, we:
- Preprocess real-world housing data
- Engineer features from date information
- Train multiple regression models
- Evaluate and compare their performance using standard metrics
- Select the most effective model for the task.
The dataset contains **414 records and 7 columns**, with no missing values.

# Problem Type
- **Machine Learning Task:** Regression.
- **Target Variable:** House price of unit area.
- **Goal:** Minimize prediction error and maximize explained variance.

# Data Preprocessing Steps
1. **Data Cleaning**
   - Verified missing values (none found)
   - Removed duplicates if present
2. **Feature Engineering**
   - Converted `Transaction date` to datetime
   - Extracted **year** and **month** as separate features
3. **Feature Scaling**
   - Scaled continuous numerical features
   - Important for distance-based and gradient-based models
4. **Train-Test Split**
   - 80% Training Data
   - 20% Testing Data
  
# Models Trained
The following regression models were trained and compared:
- **Linear Regression** (Baseline model)
- **Decision Tree Regressor**
- **Random Forest Regressor**
- **Gradient Boosting Regressor**

Each model was trained on the same training data for fair comparison.

# Evaluation Metrics
Models were evaluated on the test set using:
- **Mean Absolute Error (MAE)** – Measures average prediction error
- **R-squared (R²)** – Measures how well the model explains variance in the target

# Best Model
**Linear Regression** emerged as the best-performing model:
- Lowest MAE
- Highest R² score
- Simple, interpretable, and efficient

Despite its simplicity, it generalized better than more complex tree-based models for this dataset.

# Key Insights
- Complex models do not always outperform simpler ones
- Feature engineering (date extraction) improved performance
- Overfitting was observed in the Decision Tree model
- Ensemble models performed well but did not significantly outperform Linear Regression

# Conclusion
In this project, multiple regression models were trained and compared to predict house prices per unit area. After evaluating each model using MAE and R² metrics, Linear Regression emerged as the best-performing model, offering the lowest prediction error and strong interpretability. This demonstrates that simpler models can be highly effective when supported by proper data preprocessing and feature engineering.


