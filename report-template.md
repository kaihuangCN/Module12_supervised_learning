# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* This analysis is to show if we can model exiting borrower and loan status data to predict future potential borrower's credit worthinesss. 

* In the dataset, we have information for each of the borrower on their loan size, interest rate, borrower income, borrwer total debt, debt to income ratio, number of credit cards, number of late/missed payment, and lastly if the loan is current or in default.

* with value_count function, we see data set contains 77536 total of records, with 75036 healthy loans and 2500 bad loans. 

* In this analysis, we utilize sklearn module to do the machine learning model.
-first we break up the data set into two with one contains all loan and borrower information, the second dataset is only the loan status 
-then we further split the datasets into training set and test set for our analysis later
-then create a logistic regressional model instance, fit the training data then predict our test data
-lastly, we utilize accuracy report, confustion matrix, and classification report to evaludate the modeling results. 

* since the data set is highly inblanced between healthy and default loans, we resampled the data and did the modeling again as in the previously to see if we can achieve better prediction 

## Results


* Machine Learning Model 1:
  -Model 1 was able to predict 99.2% accuracy on the correct loan status based on the loan information 
  -0.86 for precision and 0.91 for recall and a total of average 0.88 for the F1 score



* Machine Learning Model 2:
  -Model 2 was able to predict 99.4% accuracy on the correct loan status based on the loan information,slightly higher than model 1
  -0.85 for precision and 1 for recall and a total of average 0.92 for the F1 score

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Model 2 definitely performed better than model 1 
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
Both models are with 85%-86% on precision which means we are about the same confident that each model will give us a right prediction, however model 2 had better recall value which tells that the model 2 are more likely to help us predict if loan is high risk which is what the p2p lending service is trying to identify for all of the future potential customers.
