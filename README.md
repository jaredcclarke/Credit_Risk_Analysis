# Credit_Risk_Analysis
## Overview
### Purpose
The purpose of this exercise was to use machine learning to determine credit risk. Since credit risk is inherently an unbalanced classification problem (i.e. good loans largely outweigh the riskier ones), different techniques were used to train and evaluate models in order to determine the best model for predicting credit risk for LendingClub -- a peer-to-peer lending services company.

### Resources/Tools
* Jupyter Notebook 6.0.3
* Python 3.7.9
* Anaconda 4.9.2
* LendingClub dataset `LoanStats_2019Q1.csv`
* imbalance-learn library
* scikit-learn library

## Results
### Naive Random Oversampling
* Balanced Accuracy Score: 64.0% 
* Precision (Pre) and Recall (Rec) scores for High and Low Risk:

![](https://github.com/jaredcclarke/Credit_Risk_Analysis/blob/main/Module-17-Challenge-Resources/NAR.png)

### SMOTE
* Balanced Accuracy Score: 65.1% 
* Precision (Pre) and Recall (Rec) scores for High and Low Risk:

![](https://github.com/jaredcclarke/Credit_Risk_Analysis/blob/main/Module-17-Challenge-Resources/smote.png)

### Undersampling
* Balanced Accuracy Score: 54.7% 
* Precision (Pre) and Recall (Rec) scores for High and Low Risk:

![](https://github.com/jaredcclarke/Credit_Risk_Analysis/blob/main/Module-17-Challenge-Resources/US.png)

### Combination Sampling
* Balanced Accuracy Score: 65.5% 
* Precision (Pre) and Recall (Rec) scores for High and Low Risk:

![](https://github.com/jaredcclarke/Credit_Risk_Analysis/blob/main/Module-17-Challenge-Resources/combo.png)

### Balanced Random Forest Classifier
* Balanced Accuracy Score: 78.9%
* Precision (Pre) and Recall (Rec) scores for High and Low Risk:

![](https://github.com/jaredcclarke/Credit_Risk_Analysis/blob/main/Module-17-Challenge-Resources/brfc.png)

### Easy Ensemble AdaBoost Classifier
* Balanced Accuracy Score: 93.2% 
* Precision (Pre) and Recall (Rec) scores for High and Low Risk:

![](https://github.com/jaredcclarke/Credit_Risk_Analysis/blob/main/Module-17-Challenge-Resources/eec.png)

## Summary
Based on the results, the best fitting model to determine credit risk was the Easy Ensemble Adaboost classifier because it has highest accuracy score of 93.2%, as well as the highest Precision and Recall scores. There is a high reliabilty in high risk loans actually being high risk (precision) and a high reliability in risks being correctly designated as high and low risk (recall). This is because in AdaBoost, the model is trained then evaluated. After evaluating the errors of the first model, another model is trained, but it gives extra weight to the errors from the previous model to facilitate the minimizing of similar errors in subsequent models






