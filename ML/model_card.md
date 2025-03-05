# Model Card: CatBoostRegressor for Activation Energy Prediction

## Model Overview
This model is a **CatBoostRegressor**, a machine learning model built using the CatBoost algorithm. 

## Model Information
- **Model Type**: Gradient Boosting (CatBoost)
- **Task**: Regression (Predicting Activation Energy)
- **Loss Function**: Root Mean Squared Error (RMSE)
- **Hyperparameters**:
  - **Iterations**: 900
  - **Learning Rate**: 0.083
  - **Depth**: 2
  - **Loss Function**: RMSE (Root Mean Squared Error)
  - **Silent**: True (No output during training)
  - **Subsample**: 1.0 (Full sample used for each iteration)
  - **Colsample by Level**: 0.9 (Subsample rate for each feature)
  - **Min Data in Leaf**: 9 (Minimum number of data points per leaf)

## Model Performance
The performance of the model on the validation dataset is summarized as follows:

- **R2 Score (Test)**: 0.8205
- **Mean Squared Error (Test)**: 0.1325
- **Mean Absolute Error (Test)**: 0.9094
- **R2 Score (Train)**: 0.0929

## Data
- **Input Data**: The model uses molecular and reaction features.
- **Target Variable**: Activation energy (the value being predicted by the model).

## Deployment
- **Model Format**: The model is stored as a pickle format (Ea.pkl), which can be saved and reloaded using the CatBoost library.
- **Environment**: The model requires the CatBoost library to be installed, and it should be run in a Python environment with compatible dependencies.

## Training Details
- **Training Time**: The model has been trained with 900 iterations and a learning rate of 0.083.
- **Resources**: The model was trained in an environment with the necessary hardware and software to execute the CatBoost algorithm efficiently.

## Version Information
- **CatBoost Version**: 1.2.2

---
