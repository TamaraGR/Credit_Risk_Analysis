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
![1](https://github.com/TamaraGR/Credit_Risk_Analysis/blob/main/1.png)

Above are the scores that the naive data oversampling of the datatset provided.

At 0.63 for balanced accuracy we get more than 0.36 (or 36%) of the classes as incorrect. While this predictive model carries a certain value, it certainly won't be enough in most cases. We also got an average precision score of 0.99, hense in 99% of cases this model quantified positive class predictions that do belong to the positive class. And at 0.68 our average recall score indicates that 68% of the time positive class predictions made out of all positive examples. 

### Oversampling: SMOTE
![2](https://github.com/TamaraGR/Credit_Risk_Analysis/blob/main/2.png)

Above are the scores that the SMOTE oversampling of the datatset provided. 

The balanced accuracy score is only slightly higher at 0.65, the average precision score is the same at 0.99 and the average recall score is at 0.63 (slightly lower), so the outcome is roughly the same here, and the performance of the two models is quite the same. 

### Undersampling: ClusterCentroids

![3](https://github.com/TamaraGR/Credit_Risk_Analysis/blob/main/3.png)

Above are the scores that the ClusterCentroids undersampling of the datatset provided. 

The balance accuracy score is at 52%, the average precision score is again at 99%, and the average recall score is at 45%. While this predictive model carries some value, it won't be enough in most of the times, as these scores are even lower than the ones in the oversampling models. 

### Combination of over and under-sampling models: SMOTEENN

![4](https://github.com/TamaraGR/Credit_Risk_Analysis/blob/main/4.png)

Above are the scores that the SMOTEENN combination model of the datatset provided. 

The balance accuracy score is at 62%, the average precision score is also at 99%, the average recall score is at 55%. These indicators make the combination model not the best available prediction model in this case. 

### Ensemble: Balanced Random Forest Classifier

![5](https://github.com/TamaraGR/Credit_Risk_Analysis/blob/main/5.png)

Above are the scores that the Ensemble Learner Balanced Random Forest Classifier model of the datatset provided. 

The balance accuracy score here is at 78%, the average precision score at 99% and the averae recall socre at the impressive 92%. This is by far a better prediction model than the previous ones as its prediction credibility is much higher. 

### Ensemble: Easy Ensemble AdaBoost Classifier

![6](https://github.com/TamaraGR/Credit_Risk_Analysis/blob/main/6.png)

Above are the scores that the Ensemble Learner Easy Ensemble AdaBoost Classifier model of the datatset provided. 

The balance accuracy score here is at 93%, the average precision score at 99% and the averae recall socre at the even more impressive 94%. This is the best predictive model for this dataset. 

## Analysis Summary 

We are given a dataset where the high-risk profiles are a very small portion of the data. This means that we need alearning model with the highest prediction accuracy possible for the best outcomes. The best model taht we have is the Ensemble Learner Easy Ensemble AdaBoost Classifier in this case with the highest predictability accuracy, and the second best is Ensemble Learner Balanced Random Forest Classifier model, because it also has rather high prediction scores. The oversampling, undersampling and combined models all provided rather similar and dissatisfactory results: while these learning models were somewhat useful, we couldn't rely on them in this analysis fully due to low predictability scores. 


