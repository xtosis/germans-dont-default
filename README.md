## Project Objective
Aim of this project is to find the best solution for the German loan data set which is available at:
https://archive.ics.uci.edu/ml/datasets/statlog+(german+credit+data)

## Brief Project Description 
- Binary Classification
- 20 features (Numerical, Ordinal and Nominal)
- 1000 records

## Algorithms tested so far
- Random Forests
- Gradient Boosting
- Adaptive Boosting (Decision Trees)
- Bagging (Decision Trees)
- Logistic Regression
- Linear Support Vector Machines

## Ensemble Methods
- Hard voting:  all possible odd number of combinations of aformentioned algorithms except Linear SVM
- Soft voting:  all possible number of combinations except Linear SVM
- Linear SVM could not be included in the voting ensembles as it does not provide a predict_proba_ method [under investigation]

## Methodologies
- Baysian optimization utilized instead of grid search or random search for demostration purposes and as well as to save on time while still being logical about it
- Hold-out set size: 25%
- Stratified 8 fold cross validation used to tune parameters (because I have 8 cores :P)
- Hyperparameter tuning included random state for all models until or unless varying random state siezed to have an effect on model cross validation scores except for Logistic Regression and Linear SVM models as they are not stochastic processes
- Scoring criteria: Best AUC-ROC
- All models' (stand alone and ensembles) optimal ROC threshold was found

## Feature Engineering
[To be Added]
