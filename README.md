
[![Reproducibility](https://github.com/espm-288/final-project-team-ando-shravan-final_proj/actions/workflows/main.yml/badge.svg)](ttps://github.com/espm-288/spatial-spatial_ando_shravan/actions/workflows/main.yml)

Welcome to our repository that explores datasets that would be required to build a species distribution model (SDM) for terrestrail Costa Rica. Our aim is to harmonize a bunch of datasets to the same spatial grids, such that they could be fed into a model that would then predict the some biodiversity indicator, such as species richness or Simpson's Index, etc

## Team Members:

- Ando Shah ([@ando-shah](https://github.com/ando-shah/))
- Shravan Kumar Undaru ([@undaru96](https://github.com/undaru96))

## Proposal
Find the [original proposal here](proposal.md)

## Current ToDos:

### General

- [ ] Render HTML pages
- [ ] Create a single notebook that calls functions for each of the modules
- [ ] Final output is a set of maps that shows each layer


### GBIF
- [x] Parse the GBIF stac, reduce to terrestrial Costa Rica (CR)
- [x] Gridify to some cuztomizable parameter (such as 0.01 deg lat/lon)
- [x] Work with Dask and Dask-Geopandas to parallelize processing
- [x] Establish Planetary computer workflow
- [x] Output to a rectangular geopandas dataframe
- [ ] Output to raster - GeoTIFF (geoCube did not work)
- [ ] Use groupby on lat/lon to get individual count and number of observations per grid in the final output
- [ ] Convert to a function that takes in the following:
      - gbif_data(country_code, polygon, grid_size)  


### Terra
- [ ] Define and document variables of interest
- [ ] Parallelize the function using dask
- [ ] Create grids using the helper function
- [ ] Convert into function, expand to variables of interest (beyond tmax)

### Chloris biomass


### HFI/HMI


### ESRI 10-m landcover




