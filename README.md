# Alaska IfSAR Dataset Processing for Streamline Delineation

This repository contains a Jupyter Notebook and supporting data for processing and analyzing the Alaska IfSAR dataset for streamline delineation using machine learning. The notebook demonstrates a complete workflow from data preparation to model training, using geospatial data to automatically delineate streamlines across Alaska's landscape.

---

## Repository Contents

- **notebook.ipynb**: The primary Jupyter Notebook file, titled "Alaska IfSAR Dataset Processing for Streamline Delineation," which guides you through:
  - Understanding the Alaska IfSAR dataset
  - Preprocessing and normalizing geospatial layers
  - Extracting data and label patches for machine learning
  - Training a basic convolutional neural network for streamline delineation

- **data/**: A folder containing:
  - TIFF files for various geospatial layers (e.g., elevation, topographic indices, hydrological features).
  - A reference TIFF file with labels for streamline locations.

- **Files generated in the same location as the notebook**:
  - `{huc_code}.txt`: A text file listing patch locations used for data extraction.
  - `{huc_code}_data.npy` and `{huc_code}_label.npy`: Generated data and label arrays for training.

---

## Getting Started

### Prerequisites

1. **Python 3.7+**
2. **Jupyter Notebook** or **JupyterLab**
3. Required packages (install with pip):
   ```bash
   pip install numpy matplotlib rasterio tensorflow scikit-learn

---

## Acknowledgments

- **U.S. Geological Survey (USGS)** for providing the Alaska IfSAR dataset used in this project.
- **Libraries and Tools**:
  - [NumPy](https://numpy.org/): For numerical operations and array manipulation.
  - [Matplotlib](https://matplotlib.org/): For data visualization.
  - [rasterio](https://rasterio.readthedocs.io/): For reading and handling geospatial raster data.
  - [TensorFlow](https://www.tensorflow.org/): For building and training machine learning models.

---

## Contact

For questions or suggestions, please contact **Nattapon Jaroenchai** at [nj7@illinois.edu](mailto:nj7@illinois.edu).
