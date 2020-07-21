# Machine Learning Homework
Prueba 
## Background

Auto loans, mortgages, student loans, debt consolidation ... these are just a few examples of credit and loans that people are seeking online. Peer-to-peer lending services such as LendingClub or Prosper allow investors to loan other people money without the use of a bank. However, investors always want to mitigate risk, so you have been asked by a client to help them use machine learning techniques to predict credit risk.

In this assignment, you will build and evaluate several machine-learning models to predict credit risk using free data from LendingClub. Credit risk is an inherently imbalanced classification problem (the number of good loans is much larger than the number of at-risk loans), so you will need to employ different techniques for training and evaluating models with imbalanced classes. You will use the imbalanced-learn and Scikit-learn libraries to build and evaluate models using the two following techniques:

Resampling

Ensemble Learning

## Instructions

### Resampling

You will use the imbalanced learn library to resample the LendingClub data and build and evaluate logistic regression classifiers using the resampled data.

You will:

Oversample the data using the Naive Random Oversampler and SMOTE algorithms.
Undersample the data using the Cluster Centroids algorithm.
Over- and under-sample using a combination SMOTEENN algorithm.

For each of the above, you will need to:

Train a logistic regression classifier from sklearn.linear_model using the resampled data.
Calculate the balanced accuracy score from sklearn.metrics.
Calculate the confusion matrix from sklearn.metrics.
Print the imbalanced classification report from imblearn.metrics.

Use the above to answer the following:

Which model had the best balanced accuracy score?
Which model had the best recall score?
Which model had the best geometric mean score?

### Ensemble Learning

In this section, you will train and compare two different ensemble classifiers to predict loan risk and evaluate each model. You will use the balanced random forest classifier and the easy ensemble AdaBoost classifier.
Be sure to complete the following steps for each model:

Train the model using the quarterly data from LendingClub provided in the Resource folder.
Calculate the balanced accuracy score from sklearn.metrics.
Print the confusion matrix from sklearn.metrics.
Generate a classification report using the imbalanced_classification_report from imbalanced learn.
For the balanced random forest classifier only, print the feature importance sorted in descending order (most important feature to least important) along with the feature score.

Use the above to answer the following:

Which model had the best balanced accuracy score?
Which model had the best recall score?
Which model had the best geometric mean score?
What are the top three features?

## Results

### Resampling

#### Which model had the best balanced accuracy score?

 The naive random oversampler model got the best accuracy score with a value of 0.7163

#### Which model had the best recall score?

 The naive random oversampler model got the best recall score with a value of 0.71

#### Which model had the best geometric mean score?

 The naive random oversampler model got the best geometric mean score with a value of 0.72
  
  
### Ensemble Learning 


#### Which model had the best balanced accuracy score?
  
 The Easy Ensemble Classifier model got the best accuracy score with a value of 0.9424
  
#### Which model had the best recall score?

 The Easy Ensemble Classifier model got the best recall score with a value of 0.94

#### Which model had the best geometric mean score?

 The Easy Ensemble Classifier model got the best geometric mean score with a value of 0.93

#### What are the top three features?

The top three features were (with their respective coefficient values)

total_rec_prncp - 0.09175752102205247

total_pymnt_inv - 0.06410003199501778

total_pymnt - 0.05764917485461809
