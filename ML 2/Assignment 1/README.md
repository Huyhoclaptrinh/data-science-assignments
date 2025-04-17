# Assignment 1: Distance-Weighted K-Nearest Neighbors (KNN) Classification

## Description
This project implements and evaluates a distance-weighted K-Nearest Neighbors (KNN) classifier using different distance metrics (Manhattan, Euclidean, and Chebyshev). The analysis is conducted using a Jupyter Notebook (`assignment1.ipynb`) and an HTML file (`assignment1.html`) for visualizing the results. The dataset, `knnData.csv`, contains training and test data points with features and labels for binary classification.

## Project Files
- **`assignment1.ipynb`**:
  - A Python-based Jupyter Notebook that implements the distance-weighted KNN algorithm.
  - Includes data loading, model training, prediction, and accuracy evaluation using Manhattan, Euclidean, and Chebyshev distance metrics.
  - Outputs include predictions and accuracy scores for each distance metric.
- **`assignment1.html`**:
  - A rendered HTML file showcasing the output of the Jupyter Notebook.
  - Useful for viewing the results without requiring a Jupyter environment.
- **`knnData.csv`**:
  - The dataset containing training and test data points.
  - Columns include `trainPoints_x1`, `trainPoints_x2`, `trainLabel`, `testPoints_x1`, `testPoints_x2`, and `testLabel`.

## Prerequisites
- Python 3.8+
- Jupyter Notebook
- Python Libraries:
  - `pandas`
  - `numpy`

## Setup Instructions
1. Clone the repository to your local system.
2. Install the required Python libraries using:
   ```bash
   pip install pandas numpy
   ```
3. Open the Jupyter Notebook:
   ```bash
   jupyter notebook assignment1.ipynb
   ```
4. Run the notebook cells sequentially to perform the analysis.

## Usage
- Modify the `knnData.csv` file to include updated training or test data if necessary.
- Use the notebook to experiment with different values of `k` (number of neighbors) or `p` (distance metric).
- View the `assignment1.html` file in a browser to review the analysis results.
- The notebook evaluates the KNN model with:
  - **Manhattan Distance** (p=1): Accuracy of 0.875
  - **Euclidean Distance** (p=2): Accuracy of 0.825
  - **Chebyshev Distance** (p=inf): Accuracy of 0.875

## Results Overview
The project evaluates the performance of a distance-weighted KNN classifier on a binary classification task. Key findings include:
- The classifier achieves the highest accuracy (0.875) using Manhattan and Chebyshev distance metrics.
- The Euclidean distance metric yields a slightly lower accuracy (0.825).
- The implementation uses inverse squared distance weighting to prioritize closer neighbors.

## Contribution
Feel free to submit pull requests or raise issues to improve the implementation, add new distance metrics, or enhance the analysis.