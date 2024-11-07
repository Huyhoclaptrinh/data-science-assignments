# Quarterback Rating Prediction with Multiple Linear Regression and Feature Engineering

This project uses quarterback statistics from the 2022 NFL season to predict quarterback ratings. The analysis includes building multiple linear regression models using both all available features and selected engineered features to determine model performance on a test dataset.

## Project Structure

- **assignment4.ipynb**: Jupyter notebook containing the MLR analysis, feature engineering, and model evaluation.
- **QB2022_MLR.csv**: Dataset with quarterback statistics for training the model.
- **QB2022_MLR_test.csv**: Dataset for testing the model’s predictions.

## Analysis Overview

### Part 1: Multiple Linear Regression (MLR)

1. **MLR Model with All Features**:
   - A multiple linear regression model is created to predict the rating using all features (excluding `year` and `name`) via a linear algebra approach (`inv` or `pinv` functions).
   - The model parameters are provided.

2. **MLR Model with Scikit-Learn**:
   - The same model is created using Scikit-Learn's `LinearRegression` to verify and compare the parameters with the manually computed model.

3. **Predictions on Test Set**:
   - Both models are used to predict ratings for players in `QB2022_MLR_test.csv`.
   - The mean squared error (MSE) is calculated to assess prediction accuracy.

### Part 2: Feature Engineering

Feature engineering is used to create new features to see if they improve model performance.

1. **New Feature Creation**:
   - **Cmp/Att**: Ratio of completions to attempts, calculated using the `Cmp` and `Att` columns.
   - **TD/Att**: Ratio of touchdowns to attempts, calculated using the `TD` and `Att` columns.

2. **Engineered Feature Model**:
   - A new model is created using only the features `Yds/Att`, `Cmp/Att`, and `TD/Att`.
   - The MSE of this new model is calculated on the test set to assess its performance.

3. **Model Comparison**:
   - A comparison is made between the two models to determine if the feature-engineered model outperforms the model using all original features.

## Requirements

To run this notebook, install the following Python packages:

```bash
pip install numpy pandas sklearn
```

## Instructions

1. **Open the Notebook**: Use Jupyter Notebook or JupyterLab to open `assignment4.ipynb`.
2. **Run the Analysis**:
   - Execute each cell in sequence to create the models, engineer features, make predictions, and calculate MSE.
3. **Compare Models**:
   - Examine the MSE results to determine which model performs better on the test set.

## Dataset Description

- **QB2022_MLR.csv**: Contains the training data with various performance metrics for quarterbacks.
- **QB2022_MLR_test.csv**: Contains the test data for evaluating the model.

### Columns

- **Completion Percentage**: Percentage of completed passes.
- **Cmp**: Completions.
- **Att**: Attempts.
- **TD**: Touchdowns.
- **Rating**: Quarterback rating.
- **Other Stats**: Additional columns with quarterback performance data.

## Questions Answered

- What are the parameters of the multiple linear regression model using all features?
- Does feature engineering improve the model’s prediction accuracy?
- Which model performs better: the one using all features or the one using selected engineered features?

## License

This project is provided for educational purposes.
