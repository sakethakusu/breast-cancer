Breast Cancer Classification using Machine Learning

Overview

This repository contains the implementation of machine learning models for breast cancer classification using the Breast Cancer Wisconsin (Diagnostic) dataset

The models included are:

Support Vector Machine (SVM) (primary model)

Random Forest Classifier

Gradient Boosting Classifier

Dataset

The dataset is sourced from UCI Machine Learning Repository. It contains 30 numerical features extracted from digitized images of breast masses, classified as either malignant (0) or benign (1).

Model Implementation

Data Preprocessing:

Data loading & cleaning

Feature standardization using StandardScaler

Train-test split (80%-20%)

Hyperparameter Tuning:

SVM: RandomizedSearchCV used to optimize C, kernel, and gamma

Random Forest & Gradient Boosting: GridSearchCV used to optimize hyperparameters

Evaluation Metrics:

Accuracy

Precision

Recall

F1-Score

Support Vector Machine (SVM)

Accuracy 95.61%

Precision 97.14%

Recall 95.77%

F1-Score 96.45%

Random Forest

Accuracy 96.49%

Precision 95.89%

Recall 98.59%

F1-Score 97.22%

Gradient Boosting

Accuracy 95.61%

Precision 95.83%

Recall 97.18%

F1-Score 96.50%
