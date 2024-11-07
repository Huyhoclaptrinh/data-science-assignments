# Senate Voting Records Analysis

This project analyzes voting records of 100 US senators on 46 bills (B1-B46) to explore similarities and differences in voting patterns. Key analyses include finding the senator with the closest voting record to Rhode Island senator Lincoln Chafee, identifying the senator who most disagrees with Pennsylvania senator Rick Santorum, and comparing Vermont senator Jim Jeffords to randomly selected Democratic and Republican senators.

## Project Structure

- **assignment2.ipynb**: Jupyter notebook containing code to analyze the voting records using cosine similarity.
- **senate_votes.csv**: Dataset containing voting records for each senator across 46 bills.
  - Values: `1` (Yes), `-1` (No), `0` (Abstain).
- **senate_votes_2024_extra_points.csv.xlsx**: Additional dataset from recent Senate sessions for extra credit analysis.

## Analysis Overview

1. **Closest Voting Record**:
   - Using cosine distance, we identify the senator with the closest voting pattern to Lincoln Chafee (Rhode Island).

2. **Most Disagreeing Senator**:
   - Using cosine distance, we find the senator with the most dissimilar voting pattern to Rick Santorum (Pennsylvania).

3. **Independent Senator Comparison**:
   - Vermont senator Jim Jeffords was an Independent. We compare Jeffords' voting record with 5 Democratic and 5 Republican senators selected randomly (using `random.seed(42)`), to classify him as closer to either Democrats or Republicans.

4. **Extra Credit (+10 points)**:
   - An additional dataset (`senate_votes_2024_extra_points.csv.xlsx`) provides voting records from the most recent Senate session for further comparison. This task requires formatting and analyzing this new data similarly to the main dataset.

## Requirements

To run this notebook, install the following Python packages:

```bash
pip install numpy pandas scipy
```

## Instructions

1. **Open the Notebook**: Use Jupyter Notebook or JupyterLab to open `assignment2.ipynb`.
2. **Run the Analysis**:
   - Execute each cell sequentially to carry out the comparisons and calculations.
3. **Extra Credit**:
   - For extra credit, format the `senate_votes_2024_extra_points.csv.xlsx` data similarly to `senate_votes.csv`, then repeat the analysis on the new data.

## Dataset Description

- **senate_votes.csv**: Each row represents a senator, and each column (B1-B46) represents their vote on a specific bill.
- **Values**:
  - `1`: Yes
  - `-1`: No
  - `0`: Abstain

## Questions Answered

- Who has the most similar voting record to Lincoln Chafee?
- Who disagrees the most with Rick Santorum?
- Based on voting records, is Jim Jeffords closer to the Democrats or Republicans?

## License

This project is provided for educational purposes.
