
A simple machine learning project to predict Titanic passenger survival using Decision Tree and ensemble models.

# Titanic Survival Prediction Using Ensemble Learning Techniques

## Abstract

This project presents a comparative analysis of different supervised machine learning algorithms for predicting passenger survival in the Titanic dataset. The study evaluates the performance of tree-based and ensemble-based classifiers and analyzes the impact of hyperparameter tuning on model performance.


## 1. Introduction

The objective of this study is to build classification models capable of predicting survival outcomes based on structured passenger data. The project focuses on understanding the behavior of ensemble methods compared to a single decision tree model.


## 2. Methodology

### 2.1 Data Preprocessing

The following preprocessing steps were applied:

* Removal of irrelevant attributes (`PassengerId`, `Ticket`)
* Median imputation for missing Age values
* One-hot encoding for categorical variables (Sex, Embarked)
* 80–20 train-test split for evaluation


## 3. Models Implemented

The following classifiers were implemented:

* **DecisionTreeClassifier**
* **RandomForestClassifier**
* **AdaBoostClassifier**

Additionally, hyperparameter tuning was performed on Random Forest to examine performance variation.


## 4. Results and Analysis

| Model               | Accuracy  |
| ------------------- | --------- |
| Decision Tree       | 78.2%     |
| AdaBoost            | 79.3%     |
| Random Forest       | **82.1%** |
| Tuned Random Forest | 82.1%     |

### Observations:

* Ensemble methods outperformed the single decision tree model.
* Hyperparameter tuning did not significantly alter predictive accuracy.
* The results suggest that feature engineering may have a stronger influence than model tuning for this dataset.


## 5. Conclusion

This study demonstrates that ensemble learning techniques improve classification performance on structured datasets. However, performance gains from hyperparameter tuning were limited, highlighting the importance of feature selection and engineering.


## Future Work
* Cross-validation techniques
* Comparison with additional ensemble models
