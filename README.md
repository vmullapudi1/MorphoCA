# MorphoCA

This is Morphological Cellular Automata model.
See [model.md](model.md) for information about the model.


## Requirements

- Python 3.12
- GPU with CUDA 12.4 (optional, for GPU acceleration of segmentation)

## Installation/Python environment

This project uses [Pixi](https://pixi.sh/) for environment management.

Alternately, you can open `pixi.toml` to view the python dependencies and install them into your python environment manager of choice (uv, venv, conda, etc.)

Most functionality is available in the default featureset, however if cell image viewing or segmentation is needed, the visualization environment should be used.

### 1. Install Pixi (if needed)

```bash
curl -fsSL https://pixi.sh/install.sh | bash
```

### 2. Clone the Repository

```bash
git clone <repository-url>
cd MorphoCA
```

### 3. Install Dependencies

```bash
# Install base environment
pixi install

# Optional: Install segmentation/visualization environment
pixi install --environment segmentation
#or
pixi install --environment segmentation-gpu


### 4. Activate Enviroment

```bash
# To activate the default environment
pixi shell

# To activate e.g., the visualization environment
pixi shell -e segmentation

```

The first time an .nd2 file is opened in napari, it may be slow due to the pims dependency needing to download the loci-tools.jar file for the PIMS/bioformats image loader plugin.
Make sure your JAVA_HOME environment variable is correctly set to your java installation.
