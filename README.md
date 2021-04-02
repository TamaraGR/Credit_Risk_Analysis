# Loan Prediction Risk Analysis 

## Analysis Overview 

We are performing an analysis of a dataset on credit cards credit information from a LengingClub lending services company. In this analysis on an unbalanced dataset we are using machine learning to review credit risk and perform loan prediction risk analysis. In this analysis process we have used both the data oversampling and undersampling mechanisms with SMOTE, SandomOverSampler and ClusterCentroids. Afterwards we have used oversampling and undersampling with SMOTEENN, and later on, BalancedRandomForestClassifier and EasyEnsembleClassifier.  

## Analysis Resources 

- [x] LoanStats2019 dataset (available in the repository)
- [x] imbalanced-learn documentation and scikit-learn documentation
- [x] Jupyter Notebook
- [x] Python (including dependencies, such as Numpy, Pandas, Pathlib, Collections, SKLearn, ImbalancedLearn)

## Analysis Results 

### Oversampling: Naive Random Oversampling
Below are the scores that the naive data oversampling of this datatset provided: 

At 0.63 for balanced accuracy we get more than 0.36 (or 36%) of the classes as incorrect. While this predictive model carries a certain value, it certainly won't be enough in most cases. We also got an average precision score of 0.99, hense in 99% of cases this model quantified positive class predictions that do belong to the positive class. And at 0.68 our average recall score indicates that 68% of the time positive class predictions made out of all positive examples. 




## Analysis Summary 
