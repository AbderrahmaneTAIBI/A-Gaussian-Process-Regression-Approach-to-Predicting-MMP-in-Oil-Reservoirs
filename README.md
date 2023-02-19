# A Gaussian Process Regression Approach to Predicting MMP in Oil Reservoirs

This code demonstrates the use of Gaussian Process Regression to predict the minimum miscibility pressure (MMP) in oil reservoirs. The Standing equation is used to generate synthetic data for training and testing the model. The inputs to the model are gas gravity (gg), oil API gravity (api), reservoir temperature (temp), gas specific gravity (sg_gas), and oil specific gravity (sg_oil), and the output is the MMP.

## Gaussian Process Regression (GPR)
A  probabilistic machine learning algorithm that can be used for supervised regression tasks. It is a non-parametric method that models the distribution of the target variable as a Gaussian process, which is defined by a mean function and a covariance function. GPR can be used to make predictions of the target variable for new input data by conditioning on the observed data, taking into account the uncertainty in the model's predictions. The kernel function used in GPR specifies the assumptions about the structure of the data, such as smoothness and periodicity. GPR is particularly useful for problems where there are a limited number of data points or where the data is noisy, as it can make predictions that are more robust to noise and uncertainty compared to other regression methods.

## Prerequisites
numpy
sklearn
matplotlib

## Usage
### 1- Run the script in a Python environment with the required packages installed.
### 2- The script generates synthetic data and splits it into training and testing sets.
### 3- A Gaussian Process Regression model is created and trained using the training data.
### 4- The model is used to predict the MMP for the test data.
### 5- The mean squared error and R2 score are calculated and printed.
### 6- A scatter plot of the actual MMP values vs. the predicted MMP values is displayed.

## Results
The mean squared error and R2 score for the predicted MMP values (May differ after running the model another time but they will be in the same range)  are:

Mean squared error: 2.0001716866877136e-06
R2 score: 0.8662769096105672

These results indicate that the Gaussian Process Regression model is able to accurately predict the MMP values for the test data.

