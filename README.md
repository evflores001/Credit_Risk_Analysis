# Credit_Risk_Analysis
---

## Overview of the loan prediction risk analysis:
---
The purpose of this analysis was to implement machine learning models that could predict the status of a loan, i.e., low or high risk. Using several features from the LoanStatsQ1.csv file, the features of the CSV file were used to predict the target (loan status). After creating various models with different sampling modes, the results were compared to find which model could best predict credit risk.

## Results:
---
The Results for the six tests conducted are as follow:

Naive Random Oversampling: Accuracy Score: 0.66 Pre: 0.01 Rec: 0.70 

![](https://github.com/evflores001/Credit_Risk_Analysis/blob/main/images/Oversampling.png)

SMOTE Oversample: Accuracy Score: 0.66 Pre: 0.01 Rec: 0.62 

![](https://github.com/evflores001/Credit_Risk_Analysis/blob/main/images/SMOTEoversampling.png)

Undersampling Cluster Centroids: Accuracy Score: 0.55 Pre: 0.01 Rec: 0.68 

![](https://github.com/evflores001/Credit_Risk_Analysis/blob/main/images/Oversampling.png)

Combination Over/Under SMOTEEN: Accuracy Score: 0.65 Pre: 0.01 Rec: 0.72 

![](https://github.com/evflores001/Credit_Risk_Analysis/blob/main/images/Oversampling.png)

Balanced Random Forest Classifier: Accuracy Score: 0.69 Pre: 0.88 Rec: 0.38 

![](https://github.com/evflores001/Credit_Risk_Analysis/blob/main/images/Oversampling.png)

Easy Ensemble Adaboost Classifier: Accuracy Score: 0.50 Pre: 0.33 Rec: 0.01 

![](https://github.com/evflores001/Credit_Risk_Analysis/blob/main/images/Oversampling.png)

## Summary:
---
Overall, these models shared similar values; the two models that would be the best options to implement are the Naive and and SMOTEENN models as these two have the highest recall value; in other words, these two will have a better chance of predicting fraudulent accounts even if some of the accounts may be False Negatives.

In addition, looking at the feature importances, there are some features which may not be adding much significance such as pymnt_plan_n, recoveries, hardship_flag_N, and others. Perhaps tweaking our models to exclude some of these values may aid in rendering better accuracy scores.














