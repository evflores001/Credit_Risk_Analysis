# Credit_Risk_Analysis
---

## Overview of the loan prediction risk analysis:
---
The purpose of this analysis was to implement machine learning models that could predict the status of a loan, i.e., low or high risk. Using several features from the LoanStatsQ1.csv file, the features of the CSV file were used to predict the target (loan status). After creating various models with different sampling modes, the results were compared to find which model could best predict credit risk. We tried comparing two major machine learning models, Oversampling and Undersampling models, as well as tje SMOTEENN Over- and Under-Sampling model.

## Results:
---
The Results for the six tests conducted are as follow:

### Naive Random Oversampling: 
* Accuracy Score: 65.8% 
* Precision:      High: 1% Low: 100%
* Recall:         High: 70% Low: 61%

[view image](https://github.com/evflores001/Credit_Risk_Analysis/blob/main/images/Oversampling.png)

---
### SMOTE Oversample: 
* Accuracy Score: 65.8% 
* Precision:      High: 1%  Low: 100%
* Recall:         High: 62% Low: 69%

[view image](https://github.com/evflores001/Credit_Risk_Analysis/blob/main/images/OversamplingSMOTE.png)

---
### Undersampling Cluster Centroids: 
* Accuracy Score: 54.7% 
* Precision:      High: 1%  Low: 100%
* Recall:         High: 68% Low: 41%

[view image](https://github.com/evflores001/Credit_Risk_Analysis/blob/main/images/Undersampling.png)

---
### Combination Over/Under SMOTEEN: 
* Accuracy Score: 64.8% 
* Precision:      High: 1%  Low: 100%
* Recall:         High: 72% Low: 57%

[view image](https://github.com/evflores001/Credit_Risk_Analysis/blob/main/images/SMOTEENN.png)

---
### Balanced Random Forest Classifier: 
* Accuracy Score: 68.8% 
* Precision:      High: 88% Low: 100%
* Recall:         High: 38% Low: 100%

[view image](https://github.com/evflores001/Credit_Risk_Analysis/blob/main/images/BalancedRandomForest.png)

---
### Easy Ensemble Adaboost Classifier: 
* Accuracy Score: 50.5% 
* Precision:      High: 33% Low: 99%
* Recall:         High: 1%  Low: 100% 

[view image](https://github.com/evflores001/Credit_Risk_Analysis/blob/main/images/AdaBoost.png)

## Summary:
---
Overall, these models shared similar values; the three models that would be the best options to implement are the Naive, SMOTE, and SMOTEENN models as these three have the highest recall value; in other words, these three will have a better chance of predicting fraudulent accounts even if some of the accounts may be False Negatives. Though Cluster Centroid also has a high recall value, its accuracy is close to 50%, meaning that the model is accurate only half of the time. 

In addition, looking at the feature importances, there are some features which may not be adding much significance such as pymnt_plan_n, recoveries, hardship_flag_N, and others. Perhaps tweaking our models to exclude some of these values may aid in rendering better accuracy scores.

[view image](https://github.com/evflores001/Credit_Risk_Analysis/blob/main/images/BRFfeatures.png)














