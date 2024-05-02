# Integrating machine learning in optimization of investment portfolio


# Project Description: 
We developed a neural network for constructing investment portfolios, using data from 18 key financial ratios of 100 companies to predict seasonal returns. Our approach involves ranking the predicted returns and selecting the top 25 companies to maximize portfolio performance.


# Data (2008 Q2 - 2021 Q1): 
- Independent Variable: 18 key financial ratios of 100 companies
- Dependent Variable: seasonal return of 100 companies

## Data Engineering:
- Fill missing value: utilize the average of each company to fill its own missing values.
- Create dummy variable: establish a dummy variable to distinguish if the company is government owned or not
- Check collinearity: check the correlation of each varaible and remove one of them if finding collinearity
- Normalization: Implement z-score to do normalization except *DFL* ratio

## Model (Feedforward Nerual Network):
- Number of hidden layer: 3
- activation function: sigmoid
- epoch: 50 (Use of GridSearch to find the best parameter)
- batch size: 32 (Use of GridSearch to find the best parameter)

## Final result:
The cumulative return of our selected investment portfolio is 64% higher than the market average 






