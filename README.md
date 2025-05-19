Car Evaluation using Random Forest and Other Classification Models

This repository contains the implementation of supervised machine learning models for the Car Evaluation Database. The project explores the application of Random Forest algorithm along with comparative analysis against Support Vector Machine (SVM), Decision Tree, and Logistic Regression models.
Dataset
The Car Evaluation Dataset is derived from a hierarchical decision model and contains 1728 instances with 6 categorical features:

* Cost: The buying price (vhigh, high, med, low)
* Maint: Price of maintenance (vhigh, high, med, low)
* Door: Number of doors (2, 3, 4, 5, more)
* People: Capacity in terms of persons (2, 4, more)
* Boot_size: Size of luggage boot (small, med, big)
* Safety: Estimated safety of the car (low, med, high)

The target variable Class evaluates cars as: unacceptable (unacc), acceptable (acc), good, or very good (vgood).
Implementation
The repository includes:

Data Preprocessing:

* Categorical data encoding
* Train-test split with various ratios


Random Forest Implementation:

* Default parameter model
* Random subset testing
* Feature importance analysis


Hyperparameter Tuning:

* GridSearchCV implementation
* Cross-validation


Model Comparisons:

* Random Forest (96.72% accuracy)
* Decision Tree (95.95% accuracy)
* Support Vector Machine (66.08% accuracy)
* Logistic Regression (66.08% accuracy)


Key Findings

* Random Forest achieves the highest accuracy at 96.72% with default parameters
* "Safety" feature is identified as the most important feature with a score of 0.245
* "Door" feature has the least impact with a score of 0.099
* Decision Tree performs almost as well as Random Forest
* SVM and Logistic Regression are not suitable for this categorical data

Requirements

* Python 3.x
* Scikit-learn
* Pandas
* NumPy
* Matplotlib
* Seaborn
