# Credit Risk Analysis
## Overview of the analysis

The purpose of this analysis is to evaluate the performance of six machine learning models in predicting credit risk using the credit card credit dataset from LendingClub. The dataset is imbalanced, with the majority of loans being good loans, and the minority of loans being risky loans. To address the class imbalance problem, we used resampling techniques provided by the imbalanced-learn library, including oversampling the minority class using the RandomOverSampler and SMOTE algorithms, undersampling the majority class using the ClusterCentroids algorithm, and a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. We then trained and evaluated six machine learning models, including Logistic Regression, Random Forest, Easy Ensemble AdaBoost, Balanced Random Forest, AdaBoost, and Support Vector Machine.

## Results 

### The following are the balanced accuracy scores and the precision and recall scores of all six machine learning models:

#### Naive Oversampling:
- Balanced Accuracy Score: 0.65
- Precision for high-risk loans: 0.01
- Recall for high-risk loans: 0.61
<img width="358" alt="naive" src="https://user-images.githubusercontent.com/114922260/223229876-6e4b8a5b-451c-4e5d-a7df-9a35079b7090.png">

#### SMOTE Oversampling:
- Balanced Accuracy Score: 0.62
- Precision for high-risk loans: 0.01
- Recall for high-risk loans: 0.61
<img width="369" alt="smote" src="https://user-images.githubusercontent.com/114922260/223229909-dfee7188-dd3b-4a6f-852d-3b3abaac5b58.png">

#### Undersampling:
- Balanced Accuracy Score: 0.51
- Precision for high-risk loans: 0.01
- Recall for high-risk loans: 0.60
<img width="358" alt="under" src="https://user-images.githubusercontent.com/114922260/223229941-9467af31-77e4-4a84-bf37-b2e9a5e50f4e.png">

#### Combination (Over and Under) Sampling:
- Balanced Accuracy Score: 0.64
- Precision for high-risk loans: 0.01
- Recall for high-risk loans: 0.70
<img width="365" alt="under_over" src="https://user-images.githubusercontent.com/114922260/223229993-5666b1eb-ee46-41fd-9186-b29ab9c5c06a.png">

#### Balanced Random Forest:
- Balanced Accuracy Score: 0.78
- Precision for high-risk loans: 0.04
- Recall for high-risk loans: 0.67
<img width="457" alt="forest" src="https://user-images.githubusercontent.com/114922260/223230020-a9df243d-5c97-492e-85d0-d045f4f21b13.png">

#### Easy Ensemble AdaBoost:
- Balanced Accuracy Score: 0.93
- Precision for high-risk loans: 0.07
- Recall for high-risk loans: 0.91
<img width="370" alt="ada" src="https://user-images.githubusercontent.com/114922260/223230054-65cb7932-412f-47d6-9aa5-b932aa36cde5.png">

## Summary:
The results show that the Easy Ensemble AdaBoost model had the highest balanced accuracy score of 0.93, indicating that it is the best model for predicting high-risk loans. It also had the highest precision for high-risk loans at 0.07 and the second-highest recall at 0.91.

The Balanced Random Forest model had the second-highest balanced accuracy score of 0.78 and the highest recall for high-risk loans at 0.67. However, its precision for high-risk loans was low at 0.04.

The other four models had lower balanced accuracy scores and low precision and recall for high-risk loans, making them less reliable for identifying high-risk loans.

Therefore, we recommend using the Easy Ensemble AdaBoost model for predicting high-risk loans in this dataset. However, it is important to note that the performance of this model may vary when applied to different datasets.
