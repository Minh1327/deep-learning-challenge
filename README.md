# Deep Learning Challenge Report

## Overview of the Analysis

The purpose of the analysis is to predict whether applicants will be successful if funded by Alphabet Soup based on multiple attributes including:

- `APPLICATION_TYPE` — Alphabet Soup application type
- `AFFILIATION` — Affiliated sector of industry
- `CLASSIFICATION` — Government organisation classification
- `USE_CASE` — Use case for funding
- `ORGANIZATION` — Organisation type
- `STATUS` — Active status
- `INCOME_AMT` — Income classification
- `SPECIAL_CONSIDERATIONS` — Special considerations for application
- `ASK_AMT` — Funding amount requested
- `IS_SUCCESSFUL` — Was the money used effectively

## Results

### Data Preprocessing

- `IS_SUCCESSFUL` is the target of the model. Other variables are the features of the model.
- `EIN` and `NAME` are the columns that have been removed as they would not help in predicting.

### Compiling, Training, and Evaluating the Model

- The simple model has 3 layers with 80, 30 and 1 units respectively. The first layers use `relu` as activation function and the last layer uses `sigmoid` function to produce the output of the prediction.
- The model can achieve 74% of accuracy on training data and 73% on testing data.
- For the optimisation, the training data has been increased in size to 85% of the dataset. More layers and units have been added to the neural networks and the model has been trained with more epochs. Different optimisers have been use such as `adam` and `SGD` but `adam` still performs better. Some columns have been removed as well but the model has been performed even worse.

## Summary

In summary, after many attempts to optimise the model, it seems like there is no simple method that can increase the accuracy to 75%.
