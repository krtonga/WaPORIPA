# Local Installation

To run these notebooks on your own computer, you need to create a Python environment with the required packages.

## Prerequisites

Install **Miniforge** (includes mamba, recommended):
https://github.com/conda-forge/miniforge

Or install **Miniconda**:
https://docs.conda.io/en/latest/miniconda.html

## Create the environment

From the repository root, run:

```bash
mamba env create -f environment.yml
```

This installs Python 3.10 and all required packages (numpy, rasterio, geopandas, etc.) into an environment called `waporipa`. It may take a few minutes.

## Activate the environment

```bash
conda activate waporipa
```

Your terminal prompt should show `(waporipa)` when the environment is active.

## Open a notebook

```bash
jupyter notebook
```

Or open any `.ipynb` file in VS Code and select **waporipa** as the kernel (top-right corner).

## Updating after changes to environment.yml

```bash
mamba env update -f environment.yml --prune
```

---

If you run into issues, check that you are running commands from the repository root (the folder that contains `environment.yml`).
