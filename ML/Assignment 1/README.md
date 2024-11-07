# Data Analysis on Matrices and DataFrames

This project involves analyzing and manipulating matrices and DataFrames to solve specific questions, such as identifying senators with similar voting records. Using techniques like cosine similarity, the analysis provides insights into voting similarities and patterns among U.S. senators.

## Project Structure

- **assignment1.ipynb**: Jupyter notebook containing code for data analysis and matrix operations on senator voting records.
- **assignment1.html**: HTML version of the notebook.
- **dataframesMatricesHW.html**: Supporting document for working with DataFrames and matrices.

## Dataset Description

- The dataset includes voting records of U.S. senators across various bills. Key features include:
  - **Yes**: Vote recorded as `1`
  - **No**: Vote recorded as `-1`
  - **Abstain**: Recorded as `0`

## Analysis Overview

1. **Similar Voting Records**:
   - Calculate the cosine similarity between voting records of different senators to identify close or divergent voting patterns.
   
2. **Party Affiliation Analysis**:
   - Randomly select senators from both parties to compare voting records of an Independent senator.
   - Use similarity scores to classify an Independent senator as closer to either party.

3. **Extra Analysis for Current Senate Session**:
   - Optionally, repeat analysis with recent voting data for additional insights.

## Requirements

To run this notebook, install the following packages:

```bash
pip install numpy pandas matplotlib
```

## Instructions

1. **Open the Notebook**: Use Jupyter Notebook or JupyterLab to open `assignment1.ipynb`.
2. **Run the Analysis**:
   - Execute each cell in the notebook to complete data cleaning, analysis, and visualization.

## Questions Answered

- Which senators have the closest voting record to a specified senator?
- Is an Independent senator closer in voting patterns to Democrats or Republicans?

## License

This project is provided for educational purposes.
