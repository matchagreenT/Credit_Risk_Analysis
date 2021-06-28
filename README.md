# Credit_Risk_Analysis

## Overview of the loan prediction risk analysis:

As credit risk have become a inherently unbalanced classification problem, as the loans systems are easily outnumbered by risky loans. We oversampled the dataset, provided by LendingClub, using RandomOverSampler and SMOTE algorithms and undersampled it was 
the ClusterCentroidss algorithms. We used combinational approach of over and undersampling using the SMOTEENN algorithms. We compared the two learning model machines that reduce bias; BalancedRandomForestClassifier and EasyEnsembleClassifier to predict credit risk.

## Results:

Credit Risk Resampling:

![image](https://user-images.githubusercontent.com/77694480/123563794-a511e380-d784-11eb-91ed-9bce3a7914f1.png)

- Random oversampling involves randomly selecting examples from the minority class
- With replacement, they are then added to the training dataset
- The prediction of the balanced accuracy score is quite low, sitting at 63%

![image](https://user-images.githubusercontent.com/77694480/123563907-41d48100-d785-11eb-9a2e-c76bc723b2fb.png)

- SMOTE is an oversampling technique that allows synthetic samples to be generated fo minority classes.
- The algorith helps overcome the overfitting problem posed by random oversampling.
- The prediction of the balanced accuracy score is also low, sitting at 62.5%

![image](https://user-images.githubusercontent.com/77694480/123564015-aee81680-d785-11eb-8674-ebe727d2ce77.png)

- Undersampling consists of reducing the data by eliminating examples the belongs to the majority class with the objective of equalizing number of examples of each class.
- In this case, the ClusterCentroids algorithms was used to determine the best performance compared to the other oversampling from above.

Credit Resampling Ensemble:

![image](https://user-images.githubusercontent.com/77694480/123564253-b360ff00-d786-11eb-9e4f-bf8592bb621d.png)

- Balanced random forest classifier randomly undersamples each bootstrap sample to balance with it.
- The balanced accuracy score is sitting at 80.8%

![image](https://user-images.githubusercontent.com/77694480/123564365-31250a80-d787-11eb-818b-64572a9a4092.png)

- Easy Ensemble adaboost classifier is a meta-estimator the begins by fitting a classifier on original datasets and fits additional copies on to the same classifiers
- The balanced accuracy score is sitting at 90%

## Summary: 

In results to the learning module machines for credit risk factoring, finding that random oversampling, smote and undersampling uses actual data from real people to classify and create examples to use as training data. Though the overall prediction of the balanced accuracy scores are very low because it targets individuals from the minority class. Where as, using the balanced random forest classifier and easy ensemble adaboost classifier is more creating new data and making copies to help balance out the sampling and fitting the correct classifier onto the original dataset. The balanced accuracy score sits alot high than the other three. So recommendations towards the Credit Resampling Ensemble.
