# credit-risk-classification

This script uses a dataset of historical lending activity from a peer-to-peer lending services company to build a logistic regression model that can identify the creditworthiness of borrowers.The script performs data preprocessing, splits the data into training and testing sets, trains a logistic regression model, and evaluates its performance.

## Installation

You will also need to install the following libraries:

- numpy
- pandas
- scikit-learn

## Usage

- Place the lending_data.csv file in the Resources folder.
- Run the script to process the data, train the logistic regression model, and evaluate its performance.

## Analysis breakdown

1. Read the Data: The script reads the `lending_data.csv` file into a Pandas DataFrame.
2. Separate Features and Labels: The labels (`y`) are separated from the features (`X`).
3. Split the Data: The data is split into training and testing sets using `train_test_split`.
4. Train the Model: A logistic regression model is trained using the training data.
5. Make Predictions: The model makes predictions on the testing data using `.predict()`.
6. Evaluate the Model: The model's performance is evaluated using a confusion matrix and a classification report.

## Conclusion

The logistic regression model demonstrates high accuracy in predicting both healthy and high-risk loans. It correctly identifies 99% of healthy loans and 91% of high-risk loans. While the model is highly effective overall, the identification of high-risk loans could be improved.
