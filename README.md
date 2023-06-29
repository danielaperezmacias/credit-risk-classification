# credit-risk-classification

Classifcation Report

Overview of the Analysis


Purpose of this analysis was to evaluate a model based on loan risk. The goal was to identify the "creditworthiness" of borrowers. This module took its data from a csv data frame named 'lending_data'. Within this csv, there is the columns with its corresponding data of loan_size, interest_rate, borrower_income, debt_to_income, num_of_accounts, derogatory_marks, total_debt, and loan_status. Accuracy rate was predicted twice, first creating a logistic regression model with the original data, the second with the resampled training data. 
    
When creating the logistic regression model with the original data, the following steps were used: 
•    create the y label from the "loan_status" column, and the X data frame from the remaining columns. 
•    Split the data into training and testing dataset using "train_test_split" (code: X_train, X_test, y_train, y_test = train_test_split(X, y, random_state=1). 
•    Start creating the model, using LogisticRegression. 
•    Creating and saving the prediction, by testing X_test. The accuracy scored is gotten by using the balanced_accuracy method. 
•    Afterwards, the classification report for the model is printed to be able to further assess the model. 
    For when creating the logistic regression model but with the resampled data, the following steps were used: 
•    Using the RandomOverSampler to resample the original data. 
•    A model is created again using the LogisticRegression module but using the resampled data created one step before. 
•    A prediction is created by using the testing data. 
•    The balanced accuracy score is calculated. 
•    Finally, the classification report model is printed. 
