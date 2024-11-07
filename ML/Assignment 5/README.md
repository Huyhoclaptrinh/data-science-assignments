# Landsat Image Processing with PCA

This project involves processing Landsat images using a pipeline that scales pixel values, applies PCA to reduce dimensions, and visualizes the results. The goal is to transform data from multiple wavelength bands into a single image channel.

## Project Structure

- **assignment5.ipynb**: Jupyter notebook containing the code for loading, processing, and analyzing Landsat images.
- **assignment5.html**: HTML version of the notebook for easy viewing.

## Task Overview

1. **Image Loading and Display**:
   - Load and display 5 Landsat images from different wavelength bands.
   - Display each image with its filename as the title for reference.

2. **Pipeline for Scaling and PCA**:
   - Set up a pipeline to scale pixel values linearly between 0 and 1.
   - Apply PCA to combine 5 wavelength images into a single channel.

3. **Data Analysis**:
   - Report the number of features and samples.
   - Retrieve and display PCA directions.
   - Compute the explained variance ratio for the single-channel PCA image.

4. **Pixel and Image Display**:
   - Output the value of the last pixel in the PCA-transformed image.
   - Display the new single-channel image.

## Requirements

To run this notebook, install the following Python packages:

```bash
pip install numpy pandas matplotlib sklearn
```

## Instructions

1. **Open the Notebook**: Use Jupyter Notebook or JupyterLab to open `assignment5.ipynb`.
2. **Execute Cells**:
   - Run each cell in order to load the images, apply the pipeline, and analyze the data.

## Questions Answered

- What are the number of features and samples in the dataset?
- What are the PCA directions, and what variance is explained by the single-channel image?
- What is the value of the last pixel in the processed image?

## License

This project is provided for educational purposes.
