Insurance Charges Prediction using Linear Regression
Project Overview
This project aims to predict insurance charges using a Linear Regression model. The analysis involves data cleaning, exploratory data analysis, feature engineering, model training, and evaluation.

Data Source
The dataset used is insurance.csv, which contains various personal attributes and corresponding medical insurance charges.

Methodology
Data Loading and Initial Exploration: The insurance.csv file is loaded into a pandas DataFrame, and basic information (.info(), .describe()) is displayed.
Outlier Handling: Outliers in the 'bmi' column are identified using the IQR method and clipped to ensure data quality.
Feature Engineering: Categorical features (sex, smoker, region) are converted into numerical format using one-hot encoding with pd.get_dummies().
Model Training: A Linear Regression model is trained using 'age', 'bmi', and 'smoker_yes' as features to predict 'charges'.
Model Evaluation: The model's performance is evaluated using Mean Squared Error (MSE) on both training and test datasets.
Model Saving: The trained Linear Regression model is saved as model.pkl using Python's pickle module for future use.
