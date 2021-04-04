# Credit_Risk_Analysis

## Overview of the analysis:
The purpose of this assignment was to employ different techniques to train and evaluate models with unblanced classes. We were to use imbalanced-learn and scikit-learn libraries to build and evalute models using resampling. Using the credit card dateset, we oversampled the data using the RandomOverSampler and SMOTE algorithms and undersampled the data using the ClusterCentroids algorithm. We then used a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. We were then tasked to compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. 

## Results: 

### Naive Random Oversampling
![naive_accuracy](https://github.com/echuung94/Credit_Risk_Analysis/blob/main/Resources/naive_accuracy.png)
![naive_classification](https://github.com/echuung94/Credit_Risk_Analysis/blob/main/Resources/naive_classification.png)</br>
- There is a balanced accuracy score of 65%.
- The high risk shows a precision of about 1% with a sensitivity score of 63%. 
- The low risk has a high support of 17118, with approximately 100% precision and a sensitivity score of 66%. 

### Smote Oversampling
![smote_accuracy](https://github.com/echuung94/Credit_Risk_Analysis/blob/main/Resources/smote_accuracy.png)
![smote_classification](https://github.com/echuung94/Credit_Risk_Analysis/blob/main/Resources/smote_classification.png)</br>
- The SMOTE model shows a balanced accuracy score of 63%. 
- The high risk of this model also shows a precision of 1% with 60% sensitivity.
- The high number of the low risk population results in approximately 100% precision with 66% sensitivity. 

### Undersampling 
![undersampling_accuracy](https://github.com/echuung94/Credit_Risk_Analysis/blob/main/Resources/undersampling_accuracy.png)
![undersampling_classification](https://github.com/echuung94/Credit_Risk_Analysis/blob/main/Resources/undersampling_classification.png)
- The undersampling model results with a lower balanced accuracy score of 52%. 
- The high risk population has a precision score of 1% with 60% sensitivity. 
- The lower risk population has a similar precision score of the previous models, approximately 100%, but the sensitivity score decreased to 43%. 

### Combination Sampling
![combo_accuracy](https://github.com/echuung94/Credit_Risk_Analysis/blob/main/Resources/combo_accuracy.png)
![combo_classification](https://github.com/echuung94/Credit_Risk_Analysis/blob/main/Resources/combo_classification.png)
- The combination sampling model resulted in a balanced accuracy score of 52%. 
- The high risk population shows a precision of 1% with 71% sensivitiy. The sensivity score was the highest compared to the previous oversampling/undersampling models. 
- The low risk shows a similar precision score of 100% with 58% sensitivity. 

### BalancedRandomForest Classifier 
![randomforest_accuracy](https://github.com/echuung94/Credit_Risk_Analysis/blob/main/Resources/randomforest_accuracy.png)
![randomforest_classification](https://github.com/echuung94/Credit_Risk_Analysis/blob/main/Resources/randomforest_classification.png)
- The BalancedRandomForest Classifier model resulted in balanced accuracy score of 81%. 
- The high risk population shows a precision score of 3% with 72% sensivity. 
- The lower risk shows a precision of 100% with 89% sensitivity. 

### EasyEnsemble Classifier 
![easyensemble_accuracy](https://github.com/echuung94/Credit_Risk_Analysis/blob/main/Resources/easyensemble_accuracy.png)
![easyensemble_accuracy](https://github.com/echuung94/Credit_Risk_Analysis/blob/main/Resources/easyensemble_classification.png)
- The EasyEnsemble Classifier model resulted in the highest balanced accuracy score of 92%. 
- The high risk population shows a precision of 7% with 91% sensitivity. 
- The low risk population shows 100% with 94% sensitivity. 

## Summary: 
The models that were used to perform the credit risk analysis all resulted in a weak precision score in determining if a credit risk is high. Compared to the other models, the Ensemble classifier models showed a higher precision and sensitivity score. The EasyEnsemble resulted in a sensitivity score of 91% for the high risk population, which is a more useful model in detecting all high risk credit. Although the EasyEnsemble Classifier model, shows the highest level of sensitivity, I would still not recommend any of the models to be used due to the low precision scores. With the low precision levels, many of the lower risk credits are detected as high risk credit which could deter the bank's ability to predict credit risk accurately. 
