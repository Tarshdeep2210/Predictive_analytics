1) Project Overview

Credit card fraud detection is a challenging problem because fraudulent transactions are very rare compared to normal transactions. This project focuses on improving fraud detection performance by applying different data sampling techniques and evaluating multiple machine learning models.
Dataset Description
The dataset consists of transaction-related numerical features and a target column named Class, where:
0 represents a normal transaction
1 represents a fraudulent transaction
The dataset is highly imbalanced, which can affect model performance.

2) Methodology

Data Loading & Exploration
The dataset is loaded using Pandas and explored to understand its structure and class distribution.
Feature and Target Separation
All columns except Class are used as input features, while Class is treated as the target variable.
Train–Test Split
The dataset is split into 70% training data and 30% testing data using stratified sampling to preserve class proportions.
Handling Imbalanced Data

*) The following sampling techniques are applied to the training data:

Random Over Sampling
SMOTE
Random Under Sampling
SMOTE-ENN
SMOTE-Tomek
Model Training

*)Five machine learning models are trained on the resampled data:

Logistic Regression
Decision Tree
Random Forest
Naive Bayes
Support Vector Machine (SVM)
Evaluation
Model performance is evaluated using accuracy score on the test dataset.

3) Results
Result Table

The result table shows accuracy values for each combination of sampling technique and machine learning model. It helps compare how different balancing methods affect model performance.

4) Result Graph

A bar graph is plotted using accuracy scores to visually compare model performance across different sampling techniques.

5) Conclusion

The results show that applying sampling techniques improves fraud detection accuracy. Ensemble models like Random Forest perform consistently well. Proper handling of class imbalance is essential for effective fraud detection.
