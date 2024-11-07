# Handwritten Digit Classification using SVD

This project focuses on the classification of handwritten digits, a common task in pattern recognition. The objective is to classify unknown digit images by utilizing Singular Value Decomposition (SVD) on a dataset of labeled training images. This application is particularly useful in tasks like automatic zip code reading.

## Project Structure

- **assignment6.ipynb**: Jupyter notebook containing the code for processing and classifying handwritten digits using SVD.
- **assignment6.html**: HTML version of the notebook for easy viewing.
- **digitHW.pdf**: Project document outlining the problem, dataset, methodology, and classification requirements.

## Problem Statement

The task is to classify a set of unknown digit images (test set) by comparing them with a set of known classified images (training set). The classification uses SVD on a matrix representation of each digit.

## Dataset

- **trainInput.csv**: 256x1707 matrix where each column is a 16x16 pixel grayscale image of a handwritten digit from the training set.
- **trainOutput.csv**: 1x1707 matrix containing the correct digit classification for each column in `trainInput`.
- **testInput.csv**: 256x2007 matrix where each column is a 16x16 pixel grayscale image of a handwritten digit from the test set.
- **testOutput.csv**: 1x2007 matrix containing the correct digit classification for each column in `testInput`.

## Methodology

1. **Digit Matrix Formation**:
   - For each digit, form a matrix \( A \) where each row represents an image of that digit, resulting in 10 matrices (one for each digit).

2. **Singular Value Decomposition**:
   - Perform SVD on each matrix \( A \). The right singular vectors (Vi) act as an orthogonal basis in the image space of that digit. These are referred to as "singular images."

3. **Test Image Representation**:
   - Express each test image as a linear combination of the top \( k = 20 \) singular images of each digit, forming a least-square problem \( Ax = b \).

4. **Classification**:
   - Compute the distance between each test image and its least-square approximation.
   - Classify each test image based on the smallest residual distance to a digit’s approximation.

5. **Evaluation**:
   - Calculate the overall correct classification rate and generate a confusion matrix showing classification accuracy for each digit.

## Requirements

To run this notebook, ensure you have the following Python packages installed:

```bash
pip install numpy pandas matplotlib
```

## Instructions

1. **Open the Notebook**: Use Jupyter Notebook or JupyterLab to open `assignment6.ipynb`.
2. **Execute Cells**:
   - Run each cell sequentially to preprocess the data, perform SVD, classify test images, and evaluate accuracy.

## Questions Answered

- How accurately can the model classify handwritten digits?
- What is the confusion matrix for the test set, showing classification rates for each digit?

## License

This project is provided for educational purposes.
