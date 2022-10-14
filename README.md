# Credit Risk Analysis Challenge

## Overview
In this challenge I am creating a Supervised Learning Model to assess credit risk. In this challenge I am using imbalanced-learn and scikit-learn libraries with three algorithms; RandomOverSampler, SMOTE, and ClusterCentroids. Next I will use the SMOTEENN to resample the data and use LogisticRegression classifier to make predictions and evalute the performace of the models. Finally I used the Emsemble classifiers from imblearn.ensemble with the BalancedRandomClassifier and EasyEnsembleClassifier to predict credit risk. 

### Results
- Naive OverSampling
  - Balanced Accuracy Score: 0.6293939430565123
  - Precision: high_risk-0.01, low_risk-1.00

- SMOTE OverSampling
  - Balanced Accuracy Score: 0.6277008271188627
  - Precision: high_risk-0.01, low_risk-1.00 
  
- UnderSampling
  - Balanced Accuracy Score: 0.6277008271188627
  - Precision: high_risk-0.01, low_risk-1.00 
  
- Combination
  - Balanced Accuracy Score: 0.5103017191018931
  - Precision: high_risk-0.01, low_risk-1.00

- Balanced Random Forest Classifier
  - Balanced Accuracy Score: 0.7877672625306695
  - Precision: high_risk-0.04, low_risk-1.00
  
- Easy Ensemble Classifier
  - Balanced Accuracy Score: 0.925427358175101
  - Precision: high_risk-0.07, low_risk-1.00 


#### Results
To summarize all models tested were able to calculate low risk status %100 of the time. However when using orversampling and undersampling the accuracy of predicting low_risk and high_risk was very low with the highest being Naive Over Sampling with %62.9 accuracy and the lowest being a Combination with %51 accuracy. I would reccomend the use of the Ensemble Classifier model due to it's high accuracy score of %92.5. I do believe that is the best model in the 6 tested however, I would look for additional models due to the precision for high risk predictions only being %7. When it comes to credit risk we want to be more accurate on predicting high risk applicants than low risk. There is less potential to lose and we want the high risk to be at a higher accuracy rate. 
