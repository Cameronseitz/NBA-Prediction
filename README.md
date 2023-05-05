# Team project for CSC 422

## Overview
Worked with Carter Huskinson and Carson Orejola to uncover which team statistics, such as blocks and steals, are most important for predicting season winning rates in the NBA. We used a historical data set from the 2000-01 season to 2020-21 which had the NBA team stats for that season and how many wins they received. To see how the effectiveness of these stats have changed over time, we split this dataset into four different five-year sections and made machine learning models for each. We preprocessed the data, including use of min-max scalar normalization. For each model, we used lasso regression to predict the season winning rate, given the team stats. Using 10-fold cross-validation, we tuned the hyper-parameters for each regression model to use the values which gave the lowest average RSME. To see which statistics were most important for predictions, we extracted the coefficients of the regression models and plotted them over time to see how trends have changed in the NBA's last two decades. The Python code and resulting eight-page paper with our findings can be found in this repository.

## How to Run
1. Make sure the nbaStats_cleaned.csv file is in the same directory as the notebook
2. Open the notebook through the jupyter notebook command on the command line or JupyterHub
3. Run all the cells in order
4. Some of the graphs made in the paper are via changing the x_col variable in the 2D Correlation Graphs

Original dataset from https://www.kaggle.com/datasets/mharvnek/nba-team-stats-00-to-18
