# Credit Risk Analysis
## Overview of the analysis

The purpose of this analysis is to evaluate the performance of six machine learning models in predicting credit risk using the credit card credit dataset from LendingClub. The dataset is imbalanced, with the majority of loans being good loans, and the minority of loans being risky loans. To address the class imbalance problem, we used resampling techniques provided by the imbalanced-learn library, including oversampling the minority class using the RandomOverSampler and SMOTE algorithms, undersampling the majority class using the ClusterCentroids algorithm, and a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. We then trained and evaluated six machine learning models, including Logistic Regression, Random Forest, Easy Ensemble AdaBoost, Balanced Random Forest, AdaBoost, and Support Vector Machine.

## Results 

### The following are the balanced accuracy scores and the precision and recall scores of all six machine learning models:

#### Naive Oversampling:
- Balanced Accuracy Score: 0.65
- Precision for high-risk loans: 0.01
- Recall for high-risk loans: 0.61

#### SMOTE Oversampling:
- Balanced Accuracy Score: 0.62
-Precision for high-risk loans: 0.01
-Recall for high-risk loans: 0.61

#### Undersampling:
-Balanced Accuracy Score: 0.51
-Precision for high-risk loans: 0.01
-Recall for high-risk loans: 0.60

#### Combination (Over and Under) Sampling:
-Balanced Accuracy Score: 0.64
-Precision for high-risk loans: 0.01
-Recall for high-risk loans: 0.70

#### Balanced Random Forest:
-Balanced Accuracy Score: 0.78
-Precision for high-risk loans: 0.04
-Recall for high-risk loans: 0.67

#### Easy Ensemble AdaBoost:
-Balanced Accuracy Score: 0.93
-Precision for high-risk loans: 0.07
-Recall for high-risk loans: 0.91

##Summary:
The results show that the Easy Ensemble AdaBoost model had the highest balanced accuracy score of 0.93, indicating that it is the best model for predicting high-risk loans. It also had the highest precision for high-risk loans at 0.07 and the second-highest recall at 0.91.

The Balanced Random Forest model had the second-highest balanced accuracy score of 0.78 and the highest recall for high-risk loans at 0.67. However, its precision for high-risk loans was low at 0.04.

The other four models had lower balanced accuracy scores and low precision and recall for high-risk loans, making them less reliable for identifying high-risk loans.

Therefore, we recommend using the Easy Ensemble AdaBoost model for predicting high-risk loans in this dataset. However, it is important to note that the performance of this model may vary when applied to different datasets.
