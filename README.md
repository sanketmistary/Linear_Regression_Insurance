Insurance Cost Prediction using Linear Regression
This project demonstrates a simple linear regression model to predict medical insurance costs based on various features. The notebook covers data loading, exploratory data analysis, outlier removal, feature engineering, model training, and evaluation.

Project Structure
Data Loading: The insurance.csv dataset is loaded into a pandas DataFrame.
Exploratory Data Analysis (EDA): Basic data information (df.info(), df.describe()) and BMI distribution visualizations are performed.
Data Preprocessing:
Outliers in the 'bmi' column are identified and removed using the IQR method.
Categorical features ('sex', 'smoker', 'region') are one-hot encoded.
Feature Selection: Relevant features for the model ('age', 'bmi', 'smoker_yes') are selected.
Model Training:
The data is split into training and testing sets.
A LinearRegression model from sklearn.linear_model is trained on the training data.
Model Evaluation:
The model's performance is evaluated using Mean Squared Error (MSE) on both training and testing datasets.
Model Saving: The trained linear regression model is saved using pickle for future use.
Dataset
The insurance.csv dataset contains the following columns:

age: age of primary beneficiary
sex: insurance contractor gender, female, male
bmi: Body mass index, providing an understanding of body, weights that are relatively high or low relative to height, objective index of body weight (kg / m^2) using the ratio of height to weight, ideally 18.5 to 24.9.
children: number of children covered by health insurance / number of dependents
smoker: smoking
region: residential area of beneficiary in the US, northeast, southeast, southwest, northwest.
charges: individual medical costs billed by health insurance.
Setup and Usage
To run this notebook, you will need the following Python libraries:

pandas
numpy
matplotlib
seaborn
scikit-learn
