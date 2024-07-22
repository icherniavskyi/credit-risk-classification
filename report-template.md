# Module 12 Report Template

## Overview of the Analysis

### Purpose of the Analysis

The purpose of this analysis was to predict loan status, specifically health loans and high-risk loans with logisitc regression machine learning model. Such prediction might be helpfull for financial institutions to mitigate risks, manage their portfolios, as well as decrease human hours required for this job.

### Data Description

The data used for this analysis included financial information related to various loans. The target variable y is `loan_status`. The target variable identifies the nature of the loans bieng healthy (`0`) or high-risk (`1`). The goal of the analysis was to predict target variable using all the dimension of the dataset (variables in X) and logistic regression model. 

The dataset include 9 columns (`loan_size`, `interest_rate`, `borrower_income`, `debt_to_income`, `num_of_accounts`, `derogatory_marks` and `total_debt`, `loan_status`). As was mentioned above, the analysis was tring to predict `loan_status` variable which had 75036 healty loans (`0`) and 2500 (`1`) high-risk loans.

### Stages of the machine learning process

During the machine learning process the script goes through these stages:

- Reades the csv data and transforming it to Data Frame.
- Separates the data into labels and features
- Splits the data into train and test sub datasets.
- Creates Logistic Regression model instance and fitting the train data into it.
- Makes a prediction using the testing data.
- Evaluates model's performance by creating confusion matrix and generating classification report for the model. 

### Methods Used

To predict the loans status the script uses `LogisticRegression` model. This algorithm was used to build the primary classification model to predict loan status.


## Results

After generating classification report for the model, we can observe such results:  
- Accuracy: 0.99
- Precision for Healthy Loans (0): 1.00
- Recall for Healthy Loans (0): 0.99
- F1-Score for Healthy Loans (0): 1.00
- Precision for High-Risk Loans (1): 0.85
- Recall for High-Risk Loans (1): 0.91
- F1-Score for High-Risk Loans (1): 0.88

The interpretation of the results is discussed in the summary section of this report.

## Summary

The Logistic Regression model performed exceptionally well, with an accuracy of 99%. The model's precision and recall for healthy loans were nearly perfect, with 100% and 99% accordingly. For high-risk loans, the precision was 85%, and the recall was 91%, which bost suggests overall high ability to identify high-risk loans; however, there is room for improvement in precision.

I would reccomend the logistic regrssion model for such analysis due to its high overall accuracy and strong performance metrics. However, this model might require additional adjusstments according to the business problem at hand. If for company prediction of high-risk loans is more important further refinement or additional models might be considered to enhance precision.
