# CRESST GAIA Catalog

The CRESST GAIA project relies on data sources from a number of providers: For example, in-situ precipitation stations, streamflow gauges, and seismometers. We need a convient way to visualize all these data sources on a single interactive map. Clicking stations will provide essential metadata and a link to get to more information and data from the relevant provider API. There are also various raster layers for context. Everything on this map is loaded on-demand from external sources.

## Organization
There are two notebooks in this repository:

1. create-station-inventory.ipynb

Searches Synoptic API for precipitation and streamflow stations and the IRIS APIs for seismometers


2. landing-page-map.ipynb

Creates a leaflet map and saves it to `index.html` using [Folium](https://python-visualization.github.io/folium/latest/)


## Updates
Any commit to main will re-render index.html at https://gaia-hazlab.github.io/catalog


## Acknowledgements

To render Cloud-optimized GeoTiffs we are relying on https://titiler.xyz from DevelopmentSEED
