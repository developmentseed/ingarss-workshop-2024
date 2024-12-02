# InGARSS Scaling Science Workshop 2024

Welcome to the InGARSS Scaling Science Workshop 2024 tutorial series! This Jupyter Book site contains a collection of Jupyter notebooks designed to guide you through.

## Table of Contents

- [Getting Started](#getting-started)
- [Tutorial Notebooks](#tutorial-notebooks)
  - [Notebook 1: Setup](https://colab.research.google.com/github/developmentseed/ingarss-workshop-2024/blob/main/book/docs/00_setup.ipynb)
  - [Notebook 2: STAC & Zarr](https://colab.research.google.com/github/developmentseed/ingarss-workshop-2024/blob/main/book/docs/01_stac_and_zarr.ipynb)
  - [Notebook 3: Dynamic Visualization](https://colab.research.google.com/github/developmentseed/ingarss-workshop-2024/blob/main/book/docs/02_dynamic_visualization.ipynb)
  - [Notebook 4: Raster & Vector](https://colab.research.google.com/github/developmentseed/ingarss-workshop-2024/blob/main/book/docs/03_raster_and_vector.ipynb)
- [Repository Structure](#repository-structure)
- [Contributing](#contributing)
- [License](#license)

## Getting Started

To get started with the tutorials, you can run the notebooks directly in Google Colab, which allows you to execute code without any local setup. The notebooks can either be launched from the links below or you can launch them from the rocket icon in the top right corner of the page for each of the notebook pages.

**OR**

You can also run the notebooks locally, but you will need to install the dependencies and set up a Python environment. We recommend using [uv](https://docs.astral.sh/uv/) to manage the Python environment.

Prerequisites:
Install [uv](https://docs.astral.sh/uv/getting-started/installation/)

```bash
git clone https://github.com/developmentseed/ingarss-workshop-2024.git
cd ingarss-workshop-2024
uv sync
uv run jupyter lab
```

## Tutorial Notebooks

### Notebook 1: Setup

[Open In Colab](https://colab.research.google.com/github/developmentseed/ingarss-workshop-2024/blob/main/book/docs/00_setup.ipynb)

Downloads the data into your Google Drive to be used in the other notebooks.

### Notebook 2: STAC & Zarr

[Open In Colab](https://colab.research.google.com/github/developmentseed/ingarss-workshop-2024/blob/main/book/docs/01_stac_and_zarr.ipynb)

Learn about Cloud Native Geospatial Data Formats; we will look into STAC and Zarr by using ERA5 air temperature data.

### Notebook 3: Dynamic Visualization

[Open In Colab](https://colab.research.google.com/github/developmentseed/ingarss-workshop-2024/blob/main/book/docs/02_dynamic_visualization.ipynb)

Learn to analyze & visualize time-series data using xarray and lonboard.

### Notebook 4: Raster & Vector

[Open In Colab](https://colab.research.google.com/github/developmentseed/ingarss-workshop-2024/blob/main/book/docs/03_raster_and_vector.ipynb)

Learn about STAC & Cloud Optimized GeoTIFFs.

## Repository Structure

- `book/docs/`: Contains the tutorial Jupyter notebooks.
- `book/docs/data/`: Includes dataset files used in the tutorials.
- `.python-version`: Specifies the Python version for consistency.
- `pyproject.toml`: Project configuration file.
- `uv.lock`: Dependency lock file.

## Contributing

Contributions are welcome! If you have suggestions or find issues, please open an issue or submit a pull request.

## License

This project is licensed under the MIT License.
