# vitessce-python-tutorial

Prerequisites:
- [conda](https://conda.io/projects/conda/en/latest/user-guide/install/index.html) installation
- familiarity with Python code and Jupyter notebooks
- familiarity with using the command line (e.g., installing command line tools, downloading files)

## Setup
Set up the Python environment using [`conda`](https://conda.io/projects/conda/en/latest/user-guide/install/index.html):

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

Launch JupyterLab:

```sh
jupyter lab
```

## References

Raw data:
- Transcriptomics data from https://www.covid19cellatlas.org/index.healthy.html#habib17
  - https://covid19.cog.sanger.ac.uk/habib17.processed.h5ad
- Image data from https://idr.github.io/ome-ngff-samples/
  - https://uk1s3.embassy.ebi.ac.uk/idr/zarr/v0.3/idr0040A/3491626.zarr
