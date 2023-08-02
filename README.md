# K-Nearest Neighbors (KNN) Regression Model

## Introduction
This repository contains a Jupyter notebook for a K-Nearest Neighbors (KNN) regression model. The main goal of this project was to establish a baseline using a simple KNN model and then fine-tune its parameters to find the best K parameter. The dataset used in this project is the Kaggle's House Pricing dataset. 


## KNN Regression Model
The K-Nearest Neighbors algorithm is a distance based algorithm used for both classification and regression tasks. In this project, we focus on the regression aspect.

## Establishing Baseline
We began by implementing a simple KNN regression model with default hyperparameters and a Linear regression model. The purpose of this simple models was to establish a baseline performance for comparison with the adjusted parameters model.

## Adjusting the K Parameter
After establishing the baseline, we proceeded to change the K parameter to find the optimal value that would get the best performance on the dataset. We experimented with different values of K and evaluated the model's performance using appropriate metrics.

## Results
The performance of the KNN regression models is as follows:

- Linear Model: R-squared score = 0.608
- Simple Model (K=5): R-squared score = 0.649
- Adjusted Model (Best K=11): R-squared score = 0.657

## Conclusion
Based on the results, we can observe that the modified KNN regression model outperforms the simple model by a slight margin. It achieved a higher R-squared score of 0.658 compared to the simple model's score of 0.649. Additionally, it demonstrated no signs of overfitting, indicating that the selected K parameter generalizes well to new data.

