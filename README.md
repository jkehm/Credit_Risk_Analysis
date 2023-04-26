# Credit_Risk_Analysis

### Overview
Credit Card Risk is a very difficult thing to model correctly. This is becuase it is inherently unbalanced classification problem. Overall, good loans greatly outnumber risky loans which makes it very difficult to accurately train and evaluate models. 

In this challenge we will perform 6 different models:
* Oversampling data with the **RandomOverSampler** and **SMOTE** algorithms
* Undersampling data with the **ClusterCentroids** algorithm
* Over and undersampling with the **SMOTEEN** algorithm
* And lastly, using Ensemble classifiers with **BalancedRandomForestClassifier** AND **EasyEnsembleAdaBoostClassifier**


### Results
* <ins>Naive Random Oversampling Results:</ins> From the output below we can see a Balanced accuracy score of 64.6%. For the High_risk group we have a 1% precision score and a 71% recall. Since the low_risk group has such a large population the precision score is 100%, and the recall is 58%.

![Naive Random Oversampling](https://github.com/jkehm/Credit_Risk_Analysis/blob/main/Images/naive_random_oversampling.png)

* <ins>SMOTE Oversampling:</ins> In the SMOTE Oversampling model, we had a 65.8% Balanced accuracy score. In the high_risk group we have a 1% precision score, and a 63% recall. Again, since the low_risk group has such a large population the precision score is 100%, and the recall is 68%.

![SMOTE Oversampling](https://github.com/jkehm/Credit_Risk_Analysis/blob/main/Images/SMOTE_oversampling.png)

* <ins>Undersampling:</ins> In the oversampling model, we have a 65.8% Balanced accuracy score. In the high_risk group  we have a 1% precision score, and a 69% recall. Since the low_risk group has such a large population the precision score is 100%, and the recall is 40%.

![Undersampling](https://github.com/jkehm/Credit_Risk_Analysis/blob/main/Images/undersampling.png)

* <ins>Combination (Over and Under) Sampling:</ins> In our Combination (Over and Under) Sampling model, we have a 54.4% Balanced accuracy score. In the high_risk group  we have a 1% precision score, and a 73% recall. Since the low_risk group has such a large population the precision score is 100%, and the recall is 60%.

![Combination (Over and Under) Sampling](https://github.com/jkehm/Credit_Risk_Analysis/blob/main/Images/over_under_sampling.png)

* <ins>Balanced Random Forest Classifier:</ins>* In our first ensemble algorithm, the Balanced Random Forest Classifier model, we had a balanced accuracy score of 77.5%. In the high_risk group  we have a 3% precision score, and a 67% recall. Since the low_risk group has such a large population the precision score is 100%, and the recall is 88%.

![Balanced Random Forest Classifier](https://github.com/jkehm/Credit_Risk_Analysis/blob/main/Images/balanced_random_forest_classifier.png)

* <ins>Easy Ensemble AdaBoost Classifier:</ins> In our Easy Ensemble AdBoost Classifier model, we had a balanced accuracy score of 93.2%. In the high_risk group  we have a 9% precision score, and a 92% recall. Since the low_risk group has such a large population the precision score is 100%, and the recall is 94%.

![Easy Ensemble AdaBoost Classifier](https://github.com/jkehm/Credit_Risk_Analysis/blob/main/Images/easy_ensemble_AdaBoost.png)


### Summary
All in all we saw a fairly low precision score for all six different models we used in the high_risk group. This is due to the relatively small sample size of high_risk individuals. However, we did see a vast improvement in our precision score when we used Ensemble Classifiers. Additionally, we saw a big jump in the recall for both high and low risk groups when using the Easy Ensemble AdaBoost Classifier. Therefore, I would recommend using this model going forward.
