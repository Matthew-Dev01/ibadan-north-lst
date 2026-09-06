# Project Brief : Land Surface Temperature (LST) Dynamics of Ibadan North LGA

## 1. Project Overview
Rapid urban expansion in Ibadan North Local Government Area (LGA) has altered land cover from vegetated and mixed-use surfaces to built-up, impervious surfaces. This project investigates how that land cover change relates to surface temperature patterns, as a foundation for identifying urban heat island (UHI) effects within the LGA.

## 2. Spatial Question
**How has Land Surface Temperature (LST) in Ibadan North LGA changed between 2015 and 2025, and how does this change relate to spatial patterns of land use/land cover (LULC) change?**

## 3. Study Area
**Ibadan North Local Government Area, Oyo State, Nigeria**
- Located in southwestern Nigeria, within Ibadan metropolis
- Bounded approximately by Lagelu, Akinyele, Ibadan North-East, Ibadan North-West, and Egbeda LGAs
- Approx. area: ~27 km²
- Mixed land use: institutional (University of Ibadan), residential, and commercial areas, with pockets of vegetation

## 4. Datasets Required

|  | Dataset | Purpose | Source / Link |
|---|---------|---------|----------------|
| 1 | Landsat 8/9 Collection 2 Level-2 (Surface Temperature Band ST_B10) | LST retrieval, 2015 & 2025 (dry-season, cloud-free scenes) | [USGS EarthExplorer](https://earthexplorer.usgs.gov/) |
| 2 | Landsat 8/9 Collection 2 Level-2 (Surface Reflectance, Bands 4 & 5) | NDVI derivation for emissivity correction | [USGS EarthExplorer](https://earthexplorer.usgs.gov/) |
| 3 | Sentinel-2 MSI Level-2A imagery | Supplementary LULC classification at finer resolution | [Copernicus Data Space Ecosystem](https://dataspace.copernicus.eu/) |
| 4 | Ibadan North LGA administrative boundary shapefile | Study area delineation / clipping | [Nigeria GeoData Portal (OCHA HDX)](https://data.humdata.org/dataset/cod-ab-nga) |
| 5 | Historical LULC classification (2015) for cross-validation | Reference for change detection accuracy | [Global Land Cover by ESA WorldCover](https://esa-worldcover.org/en) |
| 6 | SRTM Digital Elevation Model (30m) | Topographic correction / context | [USGS EarthExplorer – SRTM](https://earthexplorer.usgs.gov/) |
| 7 | Google Earth Engine (platform, not a dataset) | Cloud processing of Landsat/Sentinel time series | [Google Earth Engine](https://earthengine.google.com/) |

## 5. Planned Approach (brief)
1. Acquire and pre-process Landsat imagery (2015, 2025) for the study area
2. Derive NDVI and Land Surface Emissivity, then compute LST using the mono-window/split-window algorithm
3. Classify LULC for both years (built-up, vegetation, bare soil, water)
4. Overlay LST and LULC change maps to assess correlation between land cover transition and temperature change
5. Summarize findings with maps, charts, and a short interpretation
