# Module 12 Report Template

## Overview of the Analysis

The purpose of this analysis was to use supervised learning and create a model to predict the creditworthiness of borrowers. In other words, it is used to predict if a borrower has a healthy loan profile (value of 0) or a high risk profile (value of 1). These outcome figures can be found under "Loan Status" in the csv file. The outcome was assigned using a "y" variable.

Other variables that were factored into the model included: loan size, interest rate, borrower income, debt to income ratio, number of accounts, derogatory marks, and total debit. These variables were grouped together and assigned to an "X" variable.

The X and y variables were then split into two datasets: training and testing. This was completed by using the train_test_split method. 

Next, the logistic regression model was initiated and was used to fit the training data. The model was then used to make predictions against the testing data and a dataframe was generated to compare the predicted results with the actual results of the y-test data.

The final results were generated in a confusion matrix and a classification report.

The same procedure was used to predict the data using a model with oversampled data, which is also demonstrated in the Jupyter Notebook.


## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
    - Accuracy - 0.99
    - Precision - Outcome 0: 1.00 & Outcome 1: 0.85
    - Recall - Outcome 0: 0.99 & Outcome 1: 0.91
    - F1-Score: Outcome 0: 1.00 & Outcome 1: 0.88
    - Support: 19384
    

* Machine Learning Model 2:
    - Accuracy - 0.99
    - Precision - Outcome 0: 1.00 & Outcome 1: 0.84
    - Recall - Outcome 0: 0.99 & Outcome 1: 0.99
    - F1-Score: Outcome 0: 1.00 & Outcome 1: 0.91
    - Support: 19384


## Summary

After running each model, Machine Learning Model 2 performs better but only by a slight advantage. The results above show a very close comparison between each model. The outcomes for value 0 remained the same, but Model 2 performed with an f1-score of only 0.03 higher than Model 1. 

Although the results are similar, it is important to note that predicting the value 1s is extremely vital as they represent portfolios of high risk credit. Failing to successfully predict high risk can lead to financial losses and a loss of reputation of the lending company. Hence, I would still recommend to use Model 2 as it does a better job with predicting for 1s than Model 1. 
