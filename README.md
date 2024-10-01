
# Multi-Layer Perceptron for Predicting Export Value

This project implements a machine learning pipeline to predict **export value** three years ahead using agricultural, environmental, and economic data from FAOSTAT. The pipeline includes data preprocessing, exploratory data analysis, and model building using a Multi-Layer Perceptron (MLP) regressor to forecast future export values based on historical data trends.

## Project Overview

The main objective of this project is to:

- Load and preprocess multiple FAOSTAT datasets
- Build a machine learning pipeline for predicting **export values** three years into the future
- Optimize the hyperparameters of an MLP regressor using grid search and randomized search
- Evaluate the model’s performance using cross-validation

## Datasets

The project uses various FAOSTAT datasets related to agricultural and economic indicators, including:

- **Consumer Prices Indicators**
- **Crops Production Indicators**
- **Emissions**
- **Employment**
- **Exchange Rates**
- **Fertilizers Use**
- **Food Balances**
- **Food Security**
- **Food Trade**
- **Foreign Investment**
- **Land Temperature**
- **Land Use**
- **Pesticides Use**

These datasets provide a wide range of input features for predicting future export values based on past trends and economic conditions.

## Libraries Used

- **pandas**: For data loading and manipulation
- **numpy**: For numerical operations
- **matplotlib & seaborn**: For data visualization
- **scikit-learn**: For building the machine learning pipeline, including preprocessing, model selection, and evaluation
- **scipy.stats**: For statistical transformations

## Key Features

- **Data Preprocessing**: 
  - Missing value imputation
  - Feature scaling and transformation
  - One-hot encoding for categorical variables
  - Feature engineering to handle lagged features (for predicting export value 3 years ahead)
- **Machine Learning Model**: 
  - Multi-Layer Perceptron (MLP) regressor
  - Hyperparameter tuning using Grid Search and Randomized Search
  - Cross-validation with KFold to ensure model generalization
- **Performance Metrics**:
  - Mean Squared Error (MSE)
  - Mean Absolute Error (MAE)
  
The MLP model is designed to leverage both historical agricultural data and macroeconomic factors to make accurate predictions of export values for the next three years.

## Project Structure

```bash
|-- building_mlp.ipynb  # Jupyter notebook with the code implementation
|-- datasets/           # Directory containing FAOSTAT datasets
|-- README.md           # Project documentation
```

## Instructions

To run this project:

1. Clone the repository:
    ```bash
    git clone https://github.com/your-repo-url.git
    ```
2. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```
3. Open the Jupyter notebook:
    ```bash
    jupyter notebook building_mlp.ipynb
    ```

4. Follow the steps in the notebook to preprocess the data and build the MLP model.

## Model Goal

The main goal of this project is to develop an MLP regressor that predicts the **export value** for various agricultural products, three years into the future, based on historical data trends. This prediction can aid in making informed decisions regarding agricultural policy, trade strategies, and economic planning.

## Conclusion

This project illustrates the use of neural networks to predict export values based on a comprehensive dataset of agricultural and economic indicators. By optimizing the MLP model through hyperparameter tuning and cross-validation, the pipeline produces reliable forecasts that contribute to understanding and planning future agricultural export trends.

