# PHBS_TQFML-Predicting-default-of-credit-cards-clients
Team member: Yunhe Zhang(1701213157)

Background:

Credit cards are an essential tool of payment in modern society. Card holders get a convenient way of payment as well as the right of overdraft, and banks earn fees and interest. But frequently happened default of credit cards makes banks be more alert on card holders’ qualifications. Thus it is useful to identify the relationship between card holders’ characteristics and the probability of default. Research results may also be helpful for related researches on virtual credit cards such as Mayi Huabei.

Goal:

The research is aimed at finding out variables essential to predict the probability of credit cards default as well as choosing the most satisfying predictive model.

Dataset：

http://archive.ics.uci.edu/ml/datasets/default+of+credit+card+clients

Data description:

Dataset used is called default of credit card clients, chosen from UCI website. The dataset contains 30 thousand payment data from a bank in Taiwan without any missing values. The dataset describes 23 characteristics of card holders and their default payment information, which is a binary variable with value 1 for yes and 0 for no. Variable X1 describes consumers’ limit of overdraft. Variable X2 to X5 describe basic information of consumers such as age and education. Variable X6 to X11 describe consumers’ history of past 6 month payment. Variable X12 to X17 describe amount of bill statement of these 6 months. And variable X18 to X23 describe amount of previous payment of these 6 months. Finally, X24-default payment next month is the response variable that I concern most.

Methodology:

Before classification analysis, I will preprocess data at first. With no missing values and class labels have already been encoded as integer values, related steps can be omitted. But data should be standardized to center the feature columns in the form of a normal distribution. And feature selection will be completed to find out features that play the most important roles on prediction to reduce the complexity of the model and avoid the problem of overfitting.

Then classification methods such as logistic regression, support vector machines, decision tree, K-nearest neighbors, bagging and AdaBoost will be tried. K-fold cross-validation method will be used for model tuning. Finally, different models will be evaluated to find the best model. Metrics such as precision, recall, accuracy and F1-score will be used here.The technique of assigning a larger penalty to wrong predictions on the minority class may be used to deal with class imbalance because 22% of observations default versus 78% not default.
