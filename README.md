# Pangeo 1010 Tutorial for FOSS4G 2022 Annula Gathering

This repository contains the documentation and jupyter notebooks used for delivering [the tutorial on Pangeo](https://talks.osgeo.org/foss4g-2022-workshops/talk/NF8BKU/) during the [FOSS4G 2022 conference](https://2022.foss4g.org/).

<img src="tutorial/figures/pangeo_logo.png" width="180" align="Left" /></a>
<img src="tutorial/figures/EGI-ACE_logo.png" width="180" align="Right" /></a>

<br>

The content of this repository (folder `tutorial`) is rendered as an online document using [Jupyter Book](https://jupyterbook.org/en/stable/intro.html). **You can access it [here](https://pangeo-data.github.io/foss4g-2022)**.

## FOSS4G Annual International Gathering

[FOSS4G](https://foss4g.org/) stands for **Free and Open Source Software for Geospatial** and is the annual recurring global event hosted by [OSGeo](https://www.osgeo.org/), the non-profit organization that supports and promotes the collaborative development of free and open source geographic technologies and open geospatial data. 

## FOSS4G Pangeo 101 workshop

An [introduction to the Pangeo ecosystem](https://talks.osgeo.org/foss4g-2022-workshops/talk/NF8BKU/) will be provided at FOSS4G 2022 by the Pangeo Community. You will learn how to efficiently access, analyze and visualize geospatial data at scale. The workshop timeline, setup and content of the workshop are accessible via the left menu of [this webpage](https://pangeo-data.github.io/foss4g-2022).

## The Event 
A bit of context:

Start of the event 18/07/2022
Coordinates of the event: lat 43.89, lon 10.36

News on the media:
https://euroweeklynews.com/2022/07/19/fire-massarosa-lucca-italy/

## Outline
- [ ] Access data
  - [ ] Example 1 (Local): NDVI time series analysis
    - [ ] Fetch [Copernicus Global Land service analysis-ready data](https://land.copernicus.eu/global/index.html)
    - [ ] Load and analyze data with `xarray`
      - [ ] NDVI time series analysis   
    - [ ] Visualize data with `hvplot`
  - [ ] Example 2 (STAC):  Sentinel-2 Post-Fire Monitoring in Europe. See progress in `wildfires` branch.
    - [ ] Fetch [AWS Sentinel-2 Cloud-Optimized](https://registry.opendata.aws/sentinel-2-l2a-cogs/)
    - [ ] Load and analyze data with `xarray`
      - [ ] Compute dNBR
    - [ ] Visualize data with `hvplot`
  - [ ] Example 3:  Merging land and climate datasets.
    - [ ] Fetch land and climate data
    - [ ] Load and resample datasets with `xarray`
    - [ ] Visualize data with `hvplot`
- [ ] Dask basics

## Others
- [ ] How to set up environments
  - [ ] Create a Jupyter book to compile plain markdown files and executable notebooks
