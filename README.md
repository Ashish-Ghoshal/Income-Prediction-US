

# Predicting US Census Income Category with Apache Spark


## Problem Statement

In this [notebook](predict-us-census-income.ipynb), we try to predict a person's income is above or below 50K$/yr based on features such as workclass, number of years of education, occupation, relationship, marital status, hours worked per week, race, sex etc. But the catch is here we will do entirely in PySpark. We will use the most basic model of Logistic Regression here. The goal of the notebook is not to get too fancy with the choice of the Algorithms but its more on how can you achieve or at least try to achieve what you could do using scikit-learn and pandas.

## BINARY CLASSIFICATION : LOGISTIC REGRESSION

US Adult Census data relating income to social factors such as Age, Education, race etc.

The US Adult income dataset was extracted by Barry Becker from the 1994 US Census Database. The data set consists of anonymous information such as occupation, age, native country, race, capital gain, capital loss, education, work class and more. Each row is labelled as either having a salary greater than ">50K" or "<=50K".

This Data set is split into two CSV files, named `adult-training.txt` and `adult-test.txt`.

The goal here is to train a binary classifier on the training dataset to predict the column income_bracket which has two possible values ">50K" and "<=50K" and evaluate the accuracy of the classifier with the test dataset.

Note that the dataset is made up of categorical and continuous features. It also contains missing values. The categorical columns are: workclass, education, marital_status, occupation, relationship, race, gender, native_country

The continuous columns are: age, education_num, capital_gain, capital_loss, hours_per_week.

This Dataset was obtained from the UCI repository, it can be found at:

https://archive.ics.uci.edu/ml/datasets/census+income  
http://mlr.cs.umass.edu/ml/machine-learning-databases/adult/
