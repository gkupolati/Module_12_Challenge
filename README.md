# Module_12_Challenge

Credit Risk Classification

Credit risk, a key risk in loan administration, poses a classification problem that’s inherently imbalanced. This is because healthy loans easily outnumber risky loans. In this Module_12_Challenge Challenge, I used various techniques to train and evaluate models with imbalanced classes as instructed. I also used a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.

This challenge consists of the following key subsections: Splitting the Data into Training and Testing Sets, Creating a Logistic Regression Model with the Original Data and
Predicting a Logistic Regression Model with Resampled Training Data.

Splitting the Data into Training and Testing Sets involves - Reading the lending_data.csv data from the Resources folder into a Pandas DataFrame in Jupyter notebook, Creating the labels set (y) from the “loan_status” column, and then the features (X) DataFrame from the remaining columns, Checking the balance of the labels variable (y) by using the value_counts function and then Splitting the data into training and testing datasets by using train_test_split. Please note that a value of 0 in the “loan_status” column means that the loan is healthy while a value of 1 means that the loan has a high risk of defaulting.

Creating a Logistic Regression Model with the Original Data involves the following steps:Fitting a logistic regression model by using the training data (X_train and y_train),
Saving the predictions on the testing data labels by using the testing feature data (X_test) and the fitted model and then Evaluating the model’s performance by performing the following: Calculating the accuracy score of the model, Generating a confusion matrix and Printing the classification report.

Predicting a Logistic Regression Model with Resampled Training Data on the other hand involves the Use of the RandomOverSampler module from the imbalanced-learn library to resample the data and the LogisticRegression classifier and the resampled data to fit the model and make predictions before evaluation of the model’s performance such as        Calculating the accuracy score of the model, Generating a confusion matrix and then Printing the classification report.

Key questions such as  (A) how well does the logistic regression model predict both the 0 (healthy loan) and 1 (high-risk loan) labels (B)  How well did the model predict the actual fraudulent transactions? (C) How well does the logistic regression model, fit with oversampled data, predict both the 0 (healthy loan) and 1 (high-risk loan) labels?
and (D) Evaluating the effectiveness of RandomForest, BalancedRandomForest, and RandomOverSampler  for predicting the minority class of imbalanced classifier among others.
