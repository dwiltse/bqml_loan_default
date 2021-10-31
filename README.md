## Introduction

Credit card debt has risen during the pandemic, hitting a record high of $930 billion.  Delinquency rates have also risen over the same time period, up to 5.32% across all age groups [1].  Because of these factors, businesses are looking for an edge on how to obtain new customers while limiting their risk of not being paid back by customers who default on their loans.

One way to mitigate the risk is by using data to predict which customers are more likely to pay their bills based on information collected, from demographic information about the customer’s age or location, to behavioral based data such as whether they have a previous loan default.  By using this data to classify customers into risk buckets using statistical techniques like logistic regression to predict which customers will default on a loan and make credit decisions accordingly.


## Problem Statement

The business problem I am trying to solve is predicting which customers are likely to default on a credit card loan (or conversely which customers if offered credit would be most likely to pay it back).  

## How I addressed problem statement

### Data

My dataset consists of 32,582 records from a fictional credit risk dataset. There are thirteen variables with information about each borrower, including such demographic information as age, student_status, and home ownership info.  The independent variable is the loan status, which I will try to predict using the other variables or derived variables off initial variables.  

Resource:
https://www.kaggle.com/laotse/credit-risk-dataset

### Methodology

I used logistic regression since the indepedent variable is categorical and has a binary outcome.  I used Google BigQuery Machine Learning (BQML) to run the analysis using standard SQL within the Google Cloud console.

### Findings

After preparing the data for analysis, the model had an accuracy score of .864 and an roc_auc score of .867.  The default rate on the training and testing datasets was 21.5%, so the model performed better than predicting the overall percentage of defaults in the dataset.

