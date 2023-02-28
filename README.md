# Credit Risk Analysis
## Overview of the analysis

The purpose of this analysis is to evaluate the performance of six machine learning models in predicting credit risk using the credit card credit dataset from LendingClub. The dataset is imbalanced, with the majority of loans being good loans, and the minority of loans being risky loans. To address the class imbalance problem, we used resampling techniques provided by the imbalanced-learn library, including oversampling the minority class using the RandomOverSampler and SMOTE algorithms, undersampling the majority class using the ClusterCentroids algorithm, and a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. We then trained and evaluated six machine learning models, including Logistic Regression, Random Forest, Easy Ensemble AdaBoost, Balanced Random Forest, AdaBoost, and Support Vector Machine.

## Results 

