
[![Reproducibility](https://github.com/espm-288/final-project-team-ando-shravan-final_proj/actions/workflows/main.yml/badge.svg)](ttps://github.com/espm-288/spatial-spatial_ando_shravan/actions/workflows/main.yml)

Welcome to our project that explores managing datasets that would be required to build a species distribution model (SDM). We have spatially restricted ourselevs to terrestrial Costa Rica. Our aim is to harmonize a bunch of datasets to the same spatial grids, such that they could be fed into a model that would then predict the some biodiversity indicator, such as species richness or Simpson's Biodiversity Index, etc

## Team Members:

- Ando Shah ([@ando-shah](https://github.com/ando-shah/))
- Shravan Kumar Undaru ([@undaru96](https://github.com/undaru96))

## [Github Pages Link](https://espm-288.github.io/final-project-team-ando-shravan-final_proj/)

## Proposal
Find the [original proposal here](proposal.md)


## Main Files

The following is a decription of all the files relevant to this project. We were able to wrangle only the HFI, Terra Climate and GBIF datasets for this project. However, this framework can be infinitely extensible for any other datasets relevant to building an SDM, restricted to some preordained geography.

1. [Main](scripts/main.ipynb) - Harmonizes the outputs of all the datasets and we underscore some insights within those.
2. [GBIF Module](scripts/gbif.ipynb)- The Global Biodiversity Information Facility - provides this open source dataset with geolocated species taxonomic observations worldwide. Here we parse the data relevant to terrestrial Costa Rica.
3. [HFI Module](scripts/hfi.ipynb) - The Human Footprint Index is an extensively used tool for interpreting the accelerating pressure of humanity on Earth. We use the dataset provided by Patrick W Keys et al., as one of the predictors of biodiversity. Details within the notebook
4. [Terra Climate Module](scripts/terra.ipynb) - 

### Alternative Renders
In case the .ipynb files do not render on Github, you can also view the same on Jupyter's Nbviewer:
- [NB Viewer Main](https://nbviewer.org/github/espm-288/final-project-team-ando-shravan-final_proj/blob/master/scripts/main.ipynb)
- [NB Viewer GBIF](https://nbviewer.org/github/espm-288/final-project-team-ando-shravan-final_proj/blob/master/scripts/gbif.ipynb)
- [NB Viewer HFI](https://nbviewer.org/github/espm-288/final-project-team-ando-shravan-final_proj/blob/master/scripts/hfi.ipynb)
- [NB Viewer Terra](https://nbviewer.org/github/espm-288/final-project-team-ando-shravan-final_proj/blob/master/scripts/terra.ipynb)


## ToDos (Archived):

### General

- [x] Emable Github pages
- [x] Create a single notebook that calls functions for each of the modules
- [x] Grid the outputs of each module to the same grids
- [x] Final output is a geopandas frame with each column as a different feature
- [x] Correlation analysis
- [ ] Other insights


### GBIF
- [x] Parse the GBIF stac, reduce to terrestrial Costa Rica (CR)
- [x] Gridify to some cuztomizable parameter (such as 0.01 deg lat/lon)
- [x] Work with Dask and Dask-Geopandas to parallelize processing
- [x] Establish Planetary computer workflow
- [x] Output to a rectangular geopandas dataframe
- [ ] Output to raster - GeoTIFF (geoCube did not work)
- [x] Use groupby on lat/lon to get individual count and number of observations per grid in the final output
- [x] Use dask and dask_geopandas to speed up operations

### Terra
- [x] Define and document variables of interest
- [ ] Parallelize the function using dask
- [x] Create grids using the helper function


### HFI/HMI
- [x] Parse NetCDF file
- [x] Subset for CR
- [x] Save to GeoJSON 






