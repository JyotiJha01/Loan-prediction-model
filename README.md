# Loan Prediction Model Report

## Overview

The loan prediction model aims to predict the risk of loan approval based on a dataset containing information about individuals' income, age, experience, marital status, house ownership, car ownership, profession, city, state, current job years, current house years, and risk flag. The model uses machine learning algorithms to analyze these features and classify loan applications into risky or non-risky categories.

## Data Exploration and Visualization
### 1. Load the Data:
The dataset is loaded from a JSON file and converted into a pandas DataFrame for analysis.
### 2. Basic Statistics: 
Descriptive statistics such as count, mean, standard deviation, and quartiles are computed to understand the distribution and range of numerical features.
### 3. Missing Values: 
Check for missing values in the dataset. Fortunately, there are no missing values, ensuring data integrity.
### 4. Inspect Data Types: 
Differentiate between categorical and numerical columns to understand the nature of features in the dataset.
### 5. Count of Categorical Features: 
Visualize the count of categorical features to gain insights into the distribution of categorical data.
### 6.Distribution of Numerical Features: 
Visualize the distribution of numerical features to understand their spread and identify potential outliers.
### 7. Relationship Between Features and Target: 
Explore the relationship between features and the target variable (risk flag) using box plots and count plots.

## Feature Engineering
### 1. Encode Categorical Features and Scale Numerical Features: 
One-hot encode categorical features and standardize numerical features to prepare the data for model training.

## Model Building
### 1. Split the Data: 
Split the dataset into training and testing sets to evaluate model performance.

### 2. Train a Logistic Regression Model:
Train a logistic regression model to predict loan approval risk. Evaluate the model's performance using metrics such as accuracy, precision, recall, F1-score, and confusion matrix.
* Accuracy of Logistic Regression: 87.59%
* Prediction Accuracy of Logistic Regression: 12.41%
  
### 3. Train a Random Forest Model: 
Train a random forest classifier to predict loan approval risk. Evaluate the model's performance using similar metrics and visualize the ROC curve.
* Accuracy of Random Forest: 89.86%
* Prediction Accuracy of Random Forest: 10.14%
  
## Model Evaluation
**1. Make Predictions:** Use trained models to make predictions on the test set.

**2. Evaluate the Models:** Calculate accuracy, precision, recall, F1-score, mean absolute error, mean squared error, root mean squared error, and R2 score to evaluate model performance.

**3. Confusion Matrix:** Visualize the confusion matrix to understand the model's classification performance.

**4. ROC Curve:** Plot the ROC curve to assess the model's ability to distinguish between risky and non-risky loan applications.
   
## Conclusion
The loan prediction model demonstrates satisfactory performance in predicting loan approval risk. The random forest classifier outperforms the logistic regression model in terms of accuracy and F1-score, indicating its suitability for this task. However, further optimization and fine-tuning of hyperparameters could enhance the model's performance and reliability for real-world loan approval applications.
