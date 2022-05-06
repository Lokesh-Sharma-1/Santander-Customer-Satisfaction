# Santander-Customer-Satisfaction

## Introduction
Banco Santander/ Santander group is a multinational financial services company based in Madrid and Santander in Spain. Santander maintains a presence in all global financial centers as the 16th largest banking institution in the world. Customer satisfaction is a key to success in banking. Unsatisfied customers don’t stick for long and they also don’t say anything about their Dissatisfaction. So, the bank needs to identify them and resolve their issues. So, Santander group needs to identify unsatisfied customers to remain competitive in the banking sector.

## Explanation of Business Problem
The Santander Group has millions of customers and it would be impossible for them to manually identify which customers are satisfied and which customers are unsatisfied. Santander group wants to automate this process to identify unsatisfied customers.
Santander group wants to identify unsatisfied customers early on. So, that would allow them to take necessary action to make customers happy. This would provide a huge benefit to the bank because if the customer is happy then he/she will stay with the bank for a long time. The problem is that unsatisfied customer don’t say about their dissatisfaction directly. So, based on the customer's information the machine learning model should be able to predict satisfied and unsatisfied customers. There are no low latency constraints for the problem but the predictions should happen in a reasonable time.

## Machine Learning Formulation
The problem is a binary classification problem. So, the Santander group provided a dataset with 370 anonymous features and a TARGET feature which tells whether the customer is satisfied or unsatisfied. The TARGET feature with a value of 1 represents the unsatisfied customer and a value of 0 represents a satisfied customer. So, based on these 369 features (excluding ID) the task is to predict the probability that each customer in the test set is an unsatisfied customer. so, we need to build a binary classification model that classifies satisfied and unsatisfied customers.

## Dataset Description
The dataset consists of train.csv and test.csv. The train.csv consists of 370 features(including ID) and a TARGET feature. The test.csv consists of 370 features(identical to train.csv)  and no TARGET feature. The features are anonymized and their names don't give any information about the features. Only the TARGET feature gives information about customer satisfaction. The given dataset is highly imbalanced with nearly 4% of the data having a TARGET value of 1 and nearly 96% of the data having a TARGET value of 0.

## Performance Metric
The performance metrics that can be used for this problem are AUC and Cohen’s kappa. The Santander group in the Kaggle competition used AUC as the metric.
