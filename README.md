# Predicting Fraud Mobile Money Transactions

Team member: Yunhe Zhang(1701213157)

Motivation:

Mobile payment has become a convenient way of payment in our life. Transaction size has risen rapidly in recent years. But fraud transactions happen more frequently at the same time.Thus it is useful to identify the relationship between transaction’s characters and the probability of the transaction being a fraud. In this way, mobile payment platforms can detect timely and remind consumers of payment risk.

Goal:

The research is aimed at finding out the most satisfying model to predict whether a transaction is a fraud or not according to characters of the transaction.

Dataset：

https://www.kaggle.com/ntnu-testimon/paysim1/data

Data description:

Dataset used is called "Synthetic Financial Datasets For Fraud Detection", chosen from Kaggle website. The dataset contains 6,362,619 transactions. There are 11 variables in total. Variable "isFraud" is the target variable that we want to predict. Dependent variables include transaction type, amount, transaction starter's and receiver's balance account before and after transaction. The dataset is imbalanced because 99.87% of transactions are not fraud vesus 0.13% of transactions are.

Methodology:

Before classification analysis, I will preprocess data at first. I will test whether the dataset has any missing value. And string variables will be encoded as class labels. Then data will be separated into two parts--train set and test set. Last, data will be standardized to center the feature columns in the form of a normal distribution. 

In the process of modeling, three classification methods including logistics regression, random forest and KNN will be used. K-fold cross-validation method will be used for model tuning. Finally, different models will be evaluated to find the best model. Metrics such as accuracy and FPR will be used here.The technique of assigning a larger penalty to wrong predictions on the minority class may be used to deal with class imbalance problem.
