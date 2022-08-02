# foss4g-2022
Pangeo tutorial at FOSS4G 2022



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
