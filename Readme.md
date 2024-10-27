# ML Project House Price Prediction

## Overview
This repository contains an implementation of Ridge Regression, alongside the evaluation of its performance and comparison with other machine learning algorithms like Gradient Boosting Regressor, Support Vector Regressor, Random Forest, K-Neighbors Regressor, and AdaBoost Regressor. The goal is to predict target values from given features while minimizing error, with performance measured using RMSE (Root Mean Squared Error) and R² scores.

## Code Structure
The code is organized into several cells for clarity and ease of execution. Below is a brief explanation of each section:

### 1. Import Libraries
In the first cell, necessary libraries such as NumPy and `mean_squared_error` from sklearn are imported to facilitate calculations.

### 2. Manual Ridge Regression Function
This function implements the manual computation of Ridge Regression. It adds a bias term to the feature matrix and calculates the weights (theta) using the closed-form solution of Ridge Regression:

**θ = (Xᵀ * X + α * I)⁻¹ * Xᵀ * y**

Where:
- **X** is the input matrix
- **y** is the output vector
- **α** is the regularization parameter
- **I** is the identity matrix
### 3. Predictions Function
This function generates predictions for multiple alpha values by invoking the manual Ridge Regression function and storing the results in a dictionary.

### 4. Specify Alpha Values
A range of alpha values is defined, which are used to assess the impact of regularization strength on model performance.

### 5. Get Ridge Predictions
The predictions for each alpha value are obtained by calling the predictions function.

### 6. Calculate and Print Scores
For each set of predictions, the R² score and RMSE are calculated and printed. The R² score indicates the proportion of variance explained by the model, while RMSE provides a measure of the average error in the predictions.

## Results
Below are the RMSE errors and corresponding accuracy for each alpha used in the Ridge Regression model:

| Alpha     | RMSE   | R^2          |
|-----------|--------|--------------|
| 0.01      | 0.0002 | 1.0        |
| 0.1       | 0.0010 | 1.0       |
| 1.0       | 0.0092 | 0.9995        |
| 10.0      | 0.0562 | 0.9795      |
| 100.0     | 0.1172 | 0.9111       |



### Other Methods Used
The following algorithms were also implemented and their respective performances measured:

| Methods                     | RMSE       |
|-------------------------------|------------|
| Support Vector Regressor (SVR) | 0.20379    |
| Random Forest                  | 0.01066    | 
| K-Neighbors Regressor          | 0.21668    |
| AdaBoost Regressor             | 0.02386    | 
## Outputs 
![image](https://github.com/user-attachments/assets/a659baf5-6cbc-4ecd-8128-6f6b043c0970)
![image](https://github.com/user-attachments/assets/99770b30-0843-40bb-ac76-70fd252f2ff6)
![image](https://github.com/user-attachments/assets/04563786-86e7-4513-8e68-8bd170d6b7d1)
![image](https://github.com/user-attachments/assets/07668b13-364f-4b3f-9d13-a460e542766b)
![image](https://github.com/user-attachments/assets/4a7c303b-5223-4abe-814d-7bbda4334328)

## Video Demonstration

https://github.com/user-attachments/assets/05fe4cf3-ba0c-4d61-984d-e7e5ca49bc21



## Contribution
This project was made by the following contributors:

| Registration Number | Name                      |
|---------------------|---------------------------|
| RA2211003010398     | Rishav Prakash            |
| RA2211003010436     | P Karthik Manikantan      |
| RA2211003010446     | Ujan Pradhan              |
| RA2211003010464     | Krishna Chitanya          |
