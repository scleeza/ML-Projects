# Titanic-ML
 *Data Source : The dataset comes from* [Kaggle](https://www.kaggle.com/c/titanic)
 
## Quick view
__Goal__: it is trying to use passenger list (e.g. Name, Sex, Class, Age...etc) to classify one would servive or not.

__Metrics__: Accuracy 

- __Baseline:__ 
    * NaiveBayes (val_acc = 0.78)
    * Logistic (val_acc = 0.79)


- __Feature Engineering:__
    * Have age from continuous number into categorical bins
    * Use to title to verified sex/age
    * create new feature "family size" by sum up parents and childern
    * one-hot-label to categorical features, and Standarscaler() for numericals.
    
    
- __ML Models:__
    * Logistic regression (val_acc: 0.829)
    * KNN (val_acc: 0.829)
    * Decision Tree (val_acc: 0.836)
    * Random Forest (val_acc:0.831)
    * SVM (val_acc:0.829)
    * XGBoost (Val_acc:0.841)
    > All models has been finetune hyperparameters using RandomSearchCV
