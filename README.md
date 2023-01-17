# vitessce-python-tutorial

Prerequisites:
- [conda](https://conda.io/projects/conda/en/latest/user-guide/install/index.html) installation
- familiarity with Python code and Jupyter notebooks
- familiarity with using the command line (e.g., installing command line tools, downloading files)

## Setup
Set up the Python environment using conda:

```sh
conda env create -f environment.yml
```

### Image data processing (optional)

To convert image data into OME-TIFF format, you will want to install [`bftools`](https://docs.openmicroscopy.org/bio-formats/5.9.1/users/comlinetools/index.html) by unzipping it. My installation is located at `~/software/bftools`.


## Run notebooks

Activate the environment:

```sh
conda activate vitessce-tutorial-env
```

Launch JupyterLab in the sub-directory of interest:

```sh
jupyter lab --notebook-dir=./tutorials/transcriptomics
# or
jupyter lab --notebook-dir=./tutorials/imaging
# or
jupyter lab --notebook-dir=./tutorials/spatial_single_cell
# or
jupyter lab --notebook-dir=./templates
```

To download the raw data for the tutorials, run the following notebooks:

- `./tutorials/transcriptomics/raw_data/download.ipynb`
- `./tutorials/spatial_single_cell/raw_data/download.ipynb`

## Additional resources

- [Vitessce demo data processing scripts](https://github.com/vitessce/vitessce-python/tree/main/demos)

## References

Raw data:
- Transcriptomics data from https://www.covid19cellatlas.org/index.healthy.html#habib17
- Visium data from https://scanpy.readthedocs.io/en/stable/generated/scanpy.datasets.visium_sge.html#scanpy.datasets.visium_sge