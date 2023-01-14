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

Launch JupyterLab in the sub-directory of `tutorials` of interest:

```sh
jupyter lab --notebook-dir=./tutorials/imaging
```

## References

Raw data:
- Transcriptomics data from https://www.covid19cellatlas.org/index.healthy.html#habib17
  - https://covid19.cog.sanger.ac.uk/habib17.processed.h5ad
- Image data from https://idr.github.io/ome-ngff-samples/
  - https://uk1s3.embassy.ebi.ac.uk/idr/zarr/v0.3/idr0040A/3491626.zarr
- Image data from https://mcmicro.org/datasets/
  - https://mcmicro.s3.amazonaws.com/exemplars/exemplar-001.zip
- HuBMAP data:
  - https://assets.hubmapconsortium.org/a4be39d9c1606130450a011d2f1feeff/ometiff-pyramids/processedMicroscopy/VAN0012-RK-102-167-PAS_IMS_images/VAN0012-RK-102-167-PAS_IMS-registered.ome.tif?token=
  - https://portal.hubmapconsortium.org/browse/dataset/664b8227e17ee2a35a504dd8c19c2531.vitessce.json