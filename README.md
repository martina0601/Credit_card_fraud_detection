# Credit_card_fraud_detection

# Table of Contents
*	Project description
*	Problem Statement
*	Data source
*	Explanation
*	Models Used
*	Code Execution
*	Conclusion

# Project Description
Credit card fraud is the unauthorized use of someone else's credit card or credit card information to make purchases or withdraw cash. Credit card fraud is a significant financial threat for both cardholders and issuing institutions. This project aims to build a model that can analyze credit card transactions and flag potentially fraudulent activity.
# Problem Statement
 A credit card is one of the most used financial products to make online purchases and payments. Though the Credit cards can be a convenient way to manage your finances, they can also be risky.
It is important that credit card companies are able to recognize fraudulent credit card transactions so that customers are not charged for items that they did not purchase. 
The dataset contains transactions made by credit cards in September 2013 by European cardholders. This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.
The data set has also been modified with Principal Component Analysis (PCA) to maintain confidentiality. Apart from ‘time’ and ‘amount’, all the other features (V1, V2, V3, up to V28) are the principal components obtained using PCA. The feature 'time' contains the seconds elapsed between the first transaction in the data set and the subsequent transactions. The feature 'amount' is the transaction amount. The feature 'class' represents class labelling, and it takes the value 1 in cases of fraud and 0 in normal.
# Data Source
Kaggle- Credit Card Fraud Detection
# Explanation
The project code comprises several components:
* Importing Libraries: Essential libraries like NumPy, Pandas, Matplotlib, and Seaborn are imported for data handling and visualization.
*	Data Reading: The dataset is read into a Pandas DataFrame, and are checked for any missing values.
*	Exploratory Data Analysis: Analyze and understand the data to identify patterns, relationships, and trends in the data by using Descriptive Statistics and Visualizations.
*	Feature and Target Variable Identification: The features are separated from the target variable, which indicates whether a transaction is fraudulent or legitimate.
*	Model Training: The dataset is split into training and testing subsets, where a Random Forest classifier is employed for training and predicting fraudulent transaction.
*	Model-Building/Hyperparameter Tuning: This is the final step at which we can try different models and fine-tune their hyperparameters until we get the desired level of performance on the given dataset. We should try and see if we get a better model by the various sampling techniques.
*	Model Evaluation: We need to evaluate the models using appropriate evaluation metrics. Note that since the data is imbalanced it is is more important to identify which are fraudulent transactions accurately than the non-fraudulent. We need to choose an appropriate evaluation metric which reflects this business goal.

# Models Used
*	Logistic Regression
*	Random Forest
*	Decision Tree
*	XGB Classifier

# Code Execution:
*	Import the necessary libraries.
*	Load and preprocess the dataset by reading the CSV file into a DataFrame.
*	Analyze the data for missing values or inconsistencies.
*	Define your features (X) and target variable (Y), then perform a train-test split using train_test_split from scikit-learn.
*	Check all the models on the training data and predict on the test set.
*	Evaluate model performance using metrics such as accuracy, precision, recall and F1-score.

# Conclusion
a) Out of all Machine Learning Models used, Random Forest Classifier works efficiently with Maximum Accuracy of 99.99% and macro-average of F1-Score of 0.99 acheived with Oversampling technique.

b) Oversampling Techniques proved to be efficient for handling Imbalanced Datasets.

c) RandomForest, XGBoost, DecisionTree, Logistic Regression work efficiently for this Imbalanced Datasets.
