# Individual-Task-1 - Energy Consumption Prediction

This repository contains the code and analysis used for Individual Task 1 in Case Studies in Data Science.

## Project Overview

The project investigate whether machine learning can predict energy consumption using environmental and time-related variables. Two regression models were compared:
- Random Forest Regressor
- Gradient Boosting Regressor

The models were applied separately to two publicly available energy datasets.

## Datasets

### 1. Appliances Energy Prediction
Source: UCI Machine Learnign Repository

https://archive.ics.uci.edu/dataset/374/appliances+energy+prediction

This dataset contains household appliance energy use together with indoor temperature, humidity, weather and time-related variables.

### 2. Power Consumption of Tetouan City
Source: UCI Machine Learning Repository

https://archive.ics.uci.edu/dataset/849/power+consumption+of+tetouan+city

This dataset contains weather and time-related variables together with electricity consumption for three distribution zones. Zone 1 Power Consumption was used as the prediction target.

## Analysis

The notebook includes:
- data loading and inspection
- missing-value checks
- date/time preprocessing
- feature selection
- train-test splitting
- Random Forest modelling
- Gradient Boosting modelling
- MAE, RMSE and R-squared evaluation
- baseline comparisons
- feature-importance analysis
- chronological robustness checks
- visualisations of model performance and feature importance

## Main Findings
Random Forest outperformed Gradient Boosting on both datasets. Time of day was the strongest predictor in both datasets, particularly for Tetouan Zone 1 electricity consumption.

The chronological robustness checks also showed that performance was weaker when models were required to predict a later time period, highlighting limits to future-period generalisation.

## Files
- "Alinta_Energy_ML_Assignment.ipynb" - complete Python analysis
- "README.md" - Project description and dataset information
- "energydata_complete.csv" - dataset 1
- "Tetuan City power consumption.csv" - dataset 2

## Reproducibility
The two datasets used in the analysis are included in this repository. Both were obtained from the UCI Machine Learning Repository and are licensed under CC BY 4.0. The original dataset sources are linked above.
