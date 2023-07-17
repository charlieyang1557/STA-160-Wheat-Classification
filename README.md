# STA 160 - Midterm Project: Seed Report

## Introduction
This project focuses on the analysis of three common kinds of wheat: Kama, Rose, and Canadian. The goal is to find the relationship between the features of the wheat and the kind they belong to, and to identify the unique aspects of each wheat type. Various techniques are applied for data visualization, correlation analysis, and classification.

## Dataset
The dataset, obtained from the UCI machine learning repository, comprises kernels belonging to three different varieties of wheat: Kama, Rosa, and Canadian. The features of the wheat, including area, perimeter, compactness, length, width, asymmetry coefficient, and groove length, are used as inputs for the model. The species of each kind of wheat is used as the output.

## Analysis
The analysis includes a correlation plot for the seven observation variables, which shows that all correlations except for the asymmetry coefficient are positive. The area, perimeter, width, and length have the largest average correlation among all other variables.

## Main Analysis
The main analysis includes a Leave One Out Cross Validation (LOOCV) and a Grid Search with Random Forest. The LOOCV analysis shows that the model is most efficient at a polynomial degree of 5. The Grid Search with Random Forest method indicates that when bootstrap is False, and the max features of the model are limited to 6 with the number of estimators being 3, the classification model gives a final prediction accuracy of 0.952381 on the training dataset.

## Multiclass Classification
Multiclass classification was performed to achieve a more visualized result. The variables "area" and "perimeter" were chosen as the predicting variables in this classification. The result shows that the multinomial logistic regression method performs better when adding the confidence level.

## Conclusion
This study provides multiple ways to predict and analyze the data under different circumstances. The grid search with random forest provides relatively high accuracy with the training dataset, and the accuracy is about 5% lower when passing the model through the testing dataset, but it is acceptable. The multinomial logistic classification performs better than the One vs. Rest method when adding the confidence level.

## References
- The dataset used in this project can be found [here](https://archive.ics.uci.edu/ml/datasets/seeds).
