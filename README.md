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
