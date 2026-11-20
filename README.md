# MNIST PCA Visual Dashboard

![Python](https://img.shields.io/badge/Python-3.10%2B-blue)
![Machine Learning](https://img.shields.io/badge/ML-PCA-orange)
![Dataset](https://img.shields.io/badge/Dataset-MNIST-green)
![Visualization](https://img.shields.io/badge/Visualization-Plotly%20%7C%20Matplotlib-purple)

An interactive data visualization project that uses **Principal Component Analysis (PCA)** to reduce the dimensionality of the MNIST handwritten digit dataset and visualize digit patterns in two-dimensional space.

## Overview

The MNIST dataset consists of handwritten digit images from 0 to 9. Each image is represented by 784 pixel features (28 × 28 pixels), making the dataset high-dimensional.

This project applies standardization and Principal Component Analysis (PCA) to transform the original pixel features into two principal components. The reduced data is visualized through scatter plots and interactive dashboards to explore patterns, clusters, and similarities between digit classes.

## Objectives

- Load and explore the MNIST handwritten digit dataset.
- Visualize sample digit images.
- Standardize pixel feature values.
- Apply PCA to reduce 784 features to 2 principal components.
- Analyze explained variance.
- Visualize digit classes using color-coded scatter plots.
- Explore data points using interactive hover information.
- Build a visual dashboard for exploratory analysis.

## Features

- **Dataset exploration:** Display sample handwritten digit images.
- **Data preprocessing:** Standardize features using `StandardScaler`.
- **Dimensionality reduction:** Apply PCA with two components.
- **Digit visualization:** Scatter plot colored by digit class.
- **Variance analysis:** Visualize explained variance for each component.
- **Interactive exploration:** Hover over points to inspect digit labels and PCA coordinates.
- **Dashboard:** Combined visualizations and dataset statistics.
- **Export support:** Save PCA results, variance data, plots, and interactive dashboard.

## Technologies Used

| Technology | Purpose |
|---|---|
| Python | Programming language |
| NumPy | Numerical operations |
| Pandas | Data handling and analysis |
| Matplotlib | Plotting and visualization |
| Seaborn | Statistical visualization |
| Scikit-learn | Data loading, standardization, and PCA |
| Plotly | Interactive visualizations |
| mplcursors | Matplotlib hover interactions |
| Jupyter Notebook | Development environment |

## Dataset

**MNIST Handwritten Digits Dataset**

- Images: 28 × 28 grayscale pixels
- Features per image: 784
- Classes: 10 (digits 0–9)
- Total images: 70,000

The dataset is loaded using Scikit-learn's OpenML interface, with a fallback dataset loader available through Keras.

A stratified sample of 10,000 images is used for the PCA analysis to improve execution speed while maintaining the distribution of digit classes.

## Methodology

The project follows these steps:

1. Load the MNIST handwritten digit dataset.
2. Explore the dataset and visualize sample images.
3. Perform stratified sampling.
4. Standardize the pixel features using `StandardScaler`.
5. Apply PCA and retain two principal components.
6. Calculate explained variance.
7. Create digit-colored scatter plots.
8. Add interactive hover information.
9. Build the dashboard and export the results.

## PCA Visualization

PCA transforms the original high-dimensional data into a lower-dimensional representation while preserving as much variance as possible.

The two principal components are used as the X and Y coordinates of the scatter plot. Each point represents an image, and its color indicates the corresponding digit class.

The visualization helps explore the distribution and similarities between different handwritten digit classes.

## Interactive Dashboard

The dashboard provides:

- Digit distribution visualization
- Two-dimensional PCA scatter plot
- Explained variance chart
- Interactive hover information
- Digit labels and PCA coordinates

## Installation

Clone this repository:

```bash
git clone https://github.com/YOUR-USERNAME/mnist-pca-visual-dashboard.git
```

Navigate to the project directory:

```bash
cd mnist-pca-visual-dashboard
```

Install the required dependencies:

```bash
pip install -r requirements.txt
```

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open `MNIST_PCA_Visual_Dashboard.ipynb` and run the cells sequentially.

## Results

The project produces a two-dimensional PCA representation of handwritten digits, an explained variance analysis, interactive scatter plots, and downloadable analysis outputs.

The PCA visualization makes it easier to explore the relationships between handwritten digit samples and observe areas where digit classes overlap or form distinct clusters.

## Output Files

| File | Description |
|---|---|
| `mnist_pca_results.csv` | PCA coordinates and digit labels |
| `pca_explained_variance.csv` | Explained variance of the two principal components |
| `mnist_pca_dashboard.png` | Static dashboard image |
| `mnist_pca_interactive_dashboard.html` | Interactive Plotly visualization |

## Limitations

- PCA is a linear dimensionality reduction technique.
- Reducing 784 features to 2 dimensions results in information loss.
- Some digit classes may overlap in the visualization.
- The 10,000-sample subset is used to reduce computation time.
- PCA visualization does not directly represent classification accuracy.

## Future Improvements

- Compare PCA with t-SNE and UMAP.
- Add a digit classification model.
- Explore different numbers of principal components.
- Add filtering by digit class.
- Develop a web-based dashboard using Streamlit.
- Analyze reconstruction error.

## Conclusion

This project demonstrates the application of dimensionality reduction and data visualization techniques to a high-dimensional handwritten digit dataset. PCA reduces the original 784 pixel features to two dimensions, enabling visual exploration of the MNIST dataset. Interactive visualizations provide a better understanding of the patterns, similarities, and differences among digit classes.

The project highlights the role of dimensionality reduction in exploratory data analysis and machine learning.

## Author
## Purva Ghate ##

Developed as a Machine Learning and Data Visualization project.

---

If you find this project useful, feel free to star ⭐ the repository.
