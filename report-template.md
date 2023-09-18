# Module 12 Report
By Laura Faulds

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

The purpose of this analysis was to use machine learning to parse and understand a data set describing the financial situation of a group of loan applicants so that it can predict whether a given applicant is a healthy or high-risk candidate. 

 Variables such as loan size, interest rate, borrower income, and total debt were analyzed against the given applicant's loan status. Loan status was split into two categories: 0 for Healthy, and 1 for High Risk. 
 
 In our dataset, we saw that 75,036 applicants in our dataset were give a 0 status and 2500 were given a 1. Obviously, this data was heavily skewed in the 0's favour. 
 
 In our first model, we split this dataset into training and testing categories, then fit the training data into a logistic regression model. We used this logical regression model to make predictions on our testing data, then calculated its accuracy store, generated a confusion matrix and printed a classification model. 
 
 In our second model, we followed all the same steps, except that we acknowledged our dataset's heavy bias toward the 0 category, then resampled our data so that we had 56,271 instances of both 0 (Healthy) and 1 (High Risk)


## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
  
  * Accuracy: 99.18489475856377%
  * Precision Scores: Healthy Loan 1.00, High Risk Loan 0.85
  * Recall Scores: Healthy Loan 0.99, High Risk Loan 0.91
  
* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.
  
  * Accuracy: 99.38093272802311%
  * Precision Scores: Healthy Loan 1.00, High Risk Loan 0.84
  * Recall Scores: Healthy Loan 0.99, High Risk Loan 0.99
  
## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. 

Both Model 1 and Model 2 did an excellent job of predicting and identifying healthy loans. However, Model 1's ability to predict and identify high-risk loans was inferior to Model 2's. Model 2 is ultimately the better performer. 

Although Model 1's High Risk Loan Precision Score was one degree higher than Model 2's, Model 2's significant increase in High Risk Loan Recall Score is a bigger priority when it comes to the task at hand.

Falsely identifying high-risk loans as healthy loans poses the biggest threat to the bank in terms of potential financial losses. Model 2's' 99% Recall Score means that only 1% of High Risk Loans could be falsely identified as Healthy Loans, as opposed to 91% in Model 1. 

Because of this, we would recommend going with Model 2 over Model 1. 


