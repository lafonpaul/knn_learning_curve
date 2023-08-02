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

- Linear Model: R-squared score = 0.594
- Simple Model (K=5): R-squared score = 0.608
- Normalized Model (K=5): R-squared score = 0.649
- Adjusted Model (Best K=11): R-squared score = 0.657


  

## Conclusion
Based on the results, we can observe that the modified KNN regression model outperforms the normalized model by a slight margin. It achieved a higher R-squared score of 0.658 compared to the normalized model's score of 0.649. Additionally, it demonstrated no signs of overfitting, indicating that the selected K parameter generalizes well to new data.

# Final Note

We have identified a crucial factor that significantly impacted the model's performance: data normalization. The decision to apply normalization to the dataset before training the KNN regressor proved to be the most influential aspect in improving the model's accuracy.

Before normalization, the KNN regressor achieved a test score of 0.608, which indicated a moderate level of performance. However, after applying the appropriate normalization technique, we observed a substantial increase in the test score, boosting it to 0.649. This significant improvement demonstrated the necessity of preprocessing the data, especially when working with distance-based algorithms like KNN.

Since KNN relies on the distances between data points to make predictions, scaling the features allowed the algorithm to perform better, as it could now properly consider the relative importance of each feature during the computation of distances.


