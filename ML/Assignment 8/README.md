# Assignment 8: Analyzing College Data

## Description
This project involves analyzing a dataset of college statistics using data preprocessing, exploratory analysis, and inferential statistical testing.  
The analysis is conducted using a Jupyter Notebook (`assignment8.ipynb`) and an HTML file (`assignment8.html`) for visualizing the results.  
The dataset, `collegeData.csv`, includes key metrics such as costs, admissions rates, graduation rates, and college types.

## Project Files

1. **`assignment8.ipynb`**: 
   - Jupyter Notebook for data loading, cleaning, visualization, and statistical hypothesis testing.
   - Outputs include processed datasets, visual insights, and statistical test results.
   
2. **`assignment8.html`**:
   - Rendered HTML version of the notebook for convenient review without needing a Jupyter environment.
   
3. **`collegeData.csv`**:
   - Input dataset containing various metrics for multiple colleges.

## Prerequisites

- **Python 3.8+**
- **Jupyter Notebook**
- Python Libraries:
  - `pandas`
  - `matplotlib`
  - `seaborn`
  - `scipy`

### Setup Instructions
1. Clone the repository to your local system.
2. Install the required Python libraries using:
   ```bash
   pip install pandas matplotlib seaborn
   ```
3. Open the Jupyter Notebook:
   ```bash
   jupyter notebook assignment8.ipynb
   ```
4. Run the notebook cells sequentially to perform the analysis.

### Usage
- Modify the `collegeData.csv` file to include updated college statistics if necessary.
- Use the notebook to analyze trends or modify it to explore other questions.
- View the `assignment8.html` file in a browser to review the analysis.

### Results Overview
The project consists of three major analysis phases:

- **Data Preprocessing and Cleaning**:
  - Formatted and cleaned the `collegeData.csv` dataset to prepare it for analysis.

- **Exploratory Data Analysis (EDA)**:
  - Explored distributions of tuition costs, graduation rates, and admission rates.
  - Visualized differences between private and public colleges.

- **Inferential Statistical Testing**:
  - **Chi-Square Test**: Tested relationships between categorical variables, such as college type and admissions rates.
  - **Wilcoxon Rank-Sum Test**: Compared tuition costs across different groups without assuming normal distribution.
  - **Two-Sample t-Test**: Compared mean graduation rates between two groups to assess statistical significance.

This analysis provides evidence-based insights into how college type, tuition cost, and other factors influence graduation and admissions trends.

### Contribution
Feel free to submit pull requests or raise issues to improve the analysis or add new features.
