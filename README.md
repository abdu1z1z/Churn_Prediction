Customer Churn Prediction for a Telecom Company
Project Overview
This project aims to analyze a dataset of a fictional telecom company to identify key drivers of customer churn. The primary goal is to build a machine learning model that can predict which customers are most likely to leave the service. The insights and the predictive model can help the company create targeted retention strategies to reduce revenue loss.

This project was completed as a take-home assignment for Dezert.

📂 Dataset
The dataset used is the "Telco Customer Churn" dataset, which is publicly available on Kaggle. It contains customer information, subscribed services, account details, and the churn status.

Link to Dataset: Telco Customer Churn on Kaggle

📈 Project Workflow
The project followed a standard data science lifecycle:

Data Understanding & Cleaning: Understood the nature of each feature and performed essential cleaning, such as correcting data types and unifying similar categorical values.

Exploratory Data Analysis (EDA): Created visualizations (box plots, count plots, heatmaps) to discover patterns, detect outliers, and understand relationships between features and the target variable (churn).

Feature Engineering: Engineered new, more informative features (e.g., services_count) from existing data to enhance the model's predictive power.

Data Preprocessing: Prepared the data for modeling by encoding all categorical columns, splitting the data into training and testing sets, and scaling numerical features.

Model Building & Evaluation: Trained and evaluated several classification models (Logistic Regression, XGBoost, Random Forest, etc.). Addressed the class imbalance problem using class weighting techniques to improve model performance on the minority class.

Hyperparameter Tuning: Performed basic hyperparameter tuning to optimize the settings of the best-performing models.

Extracting Insights & Recommendations: Analyzed the final model's feature importances to translate technical results into actionable business recommendations.

🔑 Key Findings & Insights
The analysis revealed several key factors that strongly influence customer churn:

Contract Type is Critical: Customers on a Month-to-Month contract have a significantly higher churn rate compared to those on one-year or two-year contracts.

Customer Tenure Matters: New customers (low tenure) are far more likely to churn. Customer loyalty increases dramatically with tenure.

Payment Method Influences Churn: Customers using Electronic Check as their payment method showed a higher tendency to churn.

Lack of Support Services: Not having key services like Online Security and Tech Support is correlated with a higher probability of churning.

(Here you can add a key visualization from your project. First, save the plot as an image file, e.g., feature_importance.png, inside an images folder in your repository, then use the following Markdown.)

![Feature Importance Plot](images/feature_importance.png)

🤖 Modeling and Final Results
After comparing multiple models, including Logistic Regression, XGBoost, and Random Forest, the final recommended model was selected based on its performance on the key business metrics, especially Recall and F1-Score for the churn class.

The tuned XGBoost model provided the best balance and highest recall after hyperparameter tuning.
