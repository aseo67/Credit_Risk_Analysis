# Credit Risk Analysis
Module 17 Challenge Files
- [credit_risk_resampling.ipynb](https://github.com/aseo67/Credit_Risk_Analysis/blob/main/credit_risk_resampling.ipynb)
- [credit_risk_ensemble.ipynb](https://github.com/aseo67/Credit_Risk_Analysis/blob/main/credit_risk_ensemble.ipynb)
- [Screenshots](https://github.com/aseo67/Credit_Risk_Analysis/tree/main/Screenshots)

## Overview of Analysis
LendingClub, a peer to peer lending services company, is exploring usage of machine learning to predict credit risk. This analysis builds and evaluates several machine learning models/algorithms to predict credit risk ("high_risk" vs. "low_risk"). The models tested are:
- Naive Random Oversampling (with _RandomOverSampler_ algorithm)
- SMOTE Oversampling (with _SMOTE_ algorithm)
- Undersampling (with _ClusterCentroids_ algorithm
- Combination (Over and Under) Sampling (with _SMOTEENN_ algorithm)
- 2 additional machine learning models that reduce bias
  - Balanced Random Forest Classifier (with _BalancedRandomForestClassifier_)
  - Easy Ensemble AdaBoost Classifier (with _EasyEnsembleClassifier_)

## Results

- Naive Random Oversampling
  - Balanced Accuracy Score: ~0.65
    ![Screenshot](https://github.com/aseo67/Credit_Risk_Analysis/blob/main/Screenshots/Screenshot_RandomOversampling%20AccuracyScore.png)
  - Precision: "high_risk" = 0.01, "low_risk" = 1.00
  - Recall: "high_risk" = 0.74, "low_risk" = 0.56
    ![Screenshot](https://github.com/aseo67/Credit_Risk_Analysis/blob/main/Screenshots/Screenshot_RandomOversampling%20ClassificationReport.png)
- SMOTE Oversampling
  - Balanced Accuracy Score: ~0.65
    ![Screenshot](https://github.com/aseo67/Credit_Risk_Analysis/blob/main/Screenshots/Screenshot_SMOTE%20AccuracyScore.png)
  - Precision: "high_risk" = 0.01, "low_risk" = 1.00
  - Recall: "high_risk" = 0.62, "low_risk" = 0.69
    ![Screenshot](https://github.com/aseo67/Credit_Risk_Analysis/blob/main/Screenshots/Screenshot_SMOTE%20ClassificationReport.png)
- Undersampling
  - Balanced Accuracy Score: ~0.54
    ![Screenshot](https://github.com/aseo67/Credit_Risk_Analysis/blob/main/Screenshots/Screenshot_UnderSampling%20AccuracyScore.png)
  - Precision: "high_risk" = 0.01, "low_risk" = 1.00
  - Recall: "high_risk" = 0.69, "low_risk" = 0.40
    ![Screenshot](https://github.com/aseo67/Credit_Risk_Analysis/blob/main/Screenshots/Screenshot_UnderSampling%20ClassificationReport.png)
- SMOTEENN (Combination) Sampling
  - Balanced Accuracy Score: ~0.68
    ![Screenshot](https://github.com/aseo67/Credit_Risk_Analysis/blob/main/Screenshots/Screenshot_SMOTEENN%20AccuracyScore.png)
  - Precision: "high_risk" = 0.01, "low_risk" = 1.00
  - Recall: "high_risk" = 0.80, "low_risk" = 0.56
    ![Screenshot](https://github.com/aseo67/Credit_Risk_Analysis/blob/main/Screenshots/Screenshot_SMOTEENN%20ClassificationReport.png)
- Balanced Random Forest Classifier
  - Balanced Accuracy Score: ~0.79
    ![Screenshot](https://github.com/aseo67/Credit_Risk_Analysis/blob/main/Screenshots/Screenshot_RandomForest%20AccuracyScore.png)
  - Precision: "high_risk" = 0.03, "low_risk" = 1.00
  - Recall: "high_risk" = 0.70, "low_risk" = 0.87
    ![Screenshot](https://github.com/aseo67/Credit_Risk_Analysis/blob/main/Screenshots/Screenshot_RandomForest%20ClassificationReport.png)
- Easy Ensemble AdaBoost Classifier
  - Balanced Accuracy Score: ~0.93
    ![Screenshot](https://github.com/aseo67/Credit_Risk_Analysis/blob/main/Screenshots/Screenshot_EasyEnsemble%20AccuracyScore.png)
  - Precision: "high_risk" = 0.09, "low_risk" = 1.00
  - Recall: "high_risk" = 0.92, "low_risk" = 0.94
    ![Screenshot](https://github.com/aseo67/Credit_Risk_Analysis/blob/main/Screenshots/Screenshot_EasyEnsemble%20ClassificationReport.png)


## Summary
Of all the models tested, the **Easy Ensemble AdaBoost Classifier** produces the strongest results, with a high accuracy score of ~0.93
With either oversampling technique
_Reco on which model to use, or there's not reco with a justification_
