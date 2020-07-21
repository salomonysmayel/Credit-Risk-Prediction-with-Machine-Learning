# Credit Risk Predictions 

## Summary 

Auto loans, mortgages, student loans, debt consolidation. These are just a few examples of credit and loans that people are seeking online. Peer-to-peer lending services such as LendingClub or Prosper allow investors to loan other people money without the use of a bank. However, investors always want to mitigate risk. In the following project different machine learning techniques are used to predict credit risk.

Several machine-learning models were build and evaluated to predict credit risk using free data from LendingClub. Credit risk is an imbalanced classification problem because the number of good loans is much larger than the number of at-risk loans, so different techniques should be employed for training and evaluating models with imbalanced classes. 

The imbalanced-learn and Scikit-learn libraries were used to build and evaluate models using the techniques Resampling and Ensemble Learning:

### Resampling

The imbalanced learn library was used to resample a LendingClub data to then build and evaluate logistic regression classifiers using the resampled data in the following ways.

Oversample the data using the Naive Random Oversampler and SMOTE algorithms.

Undersample the data using the Cluster Centroids algorithm.

Over- and under-sample using a combination SMOTEENN algorithm.

For each of the above, there following steps were followed:

Logistic regression classifier training from sklearn.linear_model using the resampled data.
Calculate the balanced accuracy score from sklearn.metrics.
Calculate the confusion matrix from sklearn.metrics.
Print the imbalanced classification report from imblearn.metrics.

To answer the following:

* Which model had the best balanced accuracy score?
* Which model had the best recall score?
* Which model had the best geometric mean score?

### Ensemble Learning

For this section two ensemble classifiers were trained and compared to predict loan risk and evaluate each model, using the balanced random forest classifier and the easy ensemble AdaBoost classifier.

Following these steps for both models:

* Training the model using the quarterly data from LendingClub.
* Calculating the balanced accuracy score from sklearn.metrics.
* Printing the confusion matrix from sklearn.metrics.
* Generating a classification report using the imbalanced_classification_report from imbalanced learn.
* For the balanced random forest classifier only,  the feature importance was printed in sorted descending order (most important feature to least important) along with the feature score.

the techniques above were used to answer the following:

1) Which model had the best balanced accuracy score?

2)Which model had the best recall score?

3)Which model had the best geometric mean score?

4)What are the top three features?

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
