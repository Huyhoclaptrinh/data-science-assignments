# Quarterback Rating Prediction Model

This project analyzes the completion percentage and rating data for quarterbacks in the 2022 NFL season, aiming to predict a quarterback's rating based on their completion percentage using linear regression.

## Project Structure

- **assignment3.ipynb**: Jupyter notebook containing the analysis, model building, and evaluation.
- **QB2022.csv**: Dataset with completion percentage and rating data for quarterbacks in the 2022 NFL season.

## Analysis Overview

1. **Linear Regression Model (Manual Calculation)**:
   - A simple linear regression model is created using a linear algebra approach (`inv` or `pinv` functions) to find the model parameters. This approach calculates the weights without using a machine learning library.
   
2. **Linear Regression Model (Using Scikit-Learn)**:
   - The same linear regression model is then created using the `LinearRegression` model from Scikit-Learn, allowing a comparison of parameters with the manual approach.

3. **Prediction for Patrick Mahomes**:
   - Using both models, the notebook predicts the rating for Patrick Mahomes, given a completion percentage of 67.1%.
   
4. **Squared Error Calculation**:
   - With Mahomes' true rating of 105.2, the notebook calculates the squared error between the model’s predicted rating and the actual rating.

## Requirements

To run this notebook, install the following Python packages:

```bash
pip install numpy pandas sklearn
```

## Instructions

1. **Open the Notebook**: Use Jupyter Notebook or JupyterLab to open `assignment3.ipynb`.
2. **Run the Analysis**:
   - Execute each cell sequentially to complete the calculations, build the models, and make predictions.
3. **Compare Model Outputs**:
   - Examine the model parameters and predictions generated by both the linear algebra approach and Scikit-Learn’s `LinearRegression`.

## Dataset Description

- **QB2022.csv**: Each row represents a quarterback, with the following columns:
  - **Completion Percentage**: The percentage of passes completed by the quarterback in 2022.
  - **Rating**: The quarterback's overall rating for the 2022 season.

## Questions Answered

- What are the model parameters for predicting quarterback rating based on completion percentage?
- How does the model built using linear algebra compare to the one built using Scikit-Learn?
- What is the predicted rating for Patrick Mahomes given a completion percentage of 67.1%?
- What is the squared error between the predicted and actual rating for Mahomes?

## License

This project is provided for educational purposes.