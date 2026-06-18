# The Thwake River Basin

**Assessing the Impact of Land Use and Land Cover Changes on Hydrological Processes in the Thwake River Basin Using GIS-Based Models and Remote Sensing Techniques**

Final year research project — BSc. Geospatial Information Science and Remote Sensing
Dedan Kimathi University of Technology, Institute of Geomatics, GIS & Remote Sensing (IGGReS)
**Author:** Maweu Mwatu (E032-01-1516/2019) · **Supervisor:** Prof. Moses Murimi Ngigi · **February 2023**

---

## Overview

The Thwake River Basin is a 1,637.65 km² semi-arid catchment spanning Machakos and Makueni Counties in Kenya, home to the seasonal Thwake, Mwania, Kalusi, Maruba, Ikiwe and Kaiti rivers and the site of the proposed Thwake Multipurpose Dam. The basin has experienced declining rainfall, rapid population growth, and conversion of natural land cover to agriculture and settlement — placing increasing pressure on an already water-scarce region.

This project uses GIS-based modelling and remote sensing to quantify how that land use change is affecting the basin's hydrology, combining satellite-derived Land Use/Land Cover (LULC) classification with Soil and Water Assessment Tool (SWAT) hydrological simulation.

## Objectives

1. Simulate the hydrological processes in the Thwake River Basin using the SWAT model.
2. Perform change detection analysis of LULC using GIS and remote sensing data.
3. Assess the impact of LULC changes on the basin's hydrological processes.

## Data Sources

| Dataset | Source | Resolution |
|---|---|---|
| Digital Elevation Model (DEM) | USGS (SRTM) | 30–90 m |
| Landsat 8 OLI imagery (2013, 2017, 2021) | USGS | 30 m |
| Sentinel 2A/2B imagery (2022) | Copernicus / USGS | 20 m |
| Digital Soil Map | FAO | 1:5,000,000 |
| Hydrogeology data | Africa Groundwater Atlas | — |
| Climate / precipitation data | CHIRPS, Kenya Meteorological Dept., CFSR | Daily, 1979–2014 |

## Methodology

- **Image preprocessing:** mosaicking, clipping, and reprojection to WGS 1984 UTM Zone 37S using ERDAS Imagine, ENVI and ArcGIS 10.5.
- **LULC classification:** supervised classification into five classes — Forest, Agriculture, Bare Land, Built-Up and Water — for 2013, 2017 and 2021.
- **Accuracy assessment:** overall classification accuracy of 96–99%, with Kappa coefficients between 0.94 and 0.98 (exceeding Anderson's 85% threshold).
- **Change detection:** tabulated LULC trends and conversion statistics across the three time periods.
- **Hydrological modelling (SWAT):** watershed delineation into 6,310 sub-basins, Hydrological Response Unit (HRU) generation (land use : soil : slope threshold 5:5:5%), weather data simulation, and a 10-year model run (2013–2022) with a 5-year warm-up period, producing daily/monthly/annual stream flow-in and flow-out results.

## Key Findings

| Land Use Class | 2013 % Cover | 2017 % Cover | 2021 % Cover | Trend |
|---|---|---|---|---|
| Agriculture | 37.37% | 37.39% | 39.15% | ▲ Positive |
| Forest | 1.91% | 5.76% | 17.57% | ▲ Positive |
| Bare Land | 7.77% | 6.16% | 6.72% | ▼ Negative |
| Built-Up | 46.42% | 50.54% | 36.52% | ▼ Negative |
| Water | 6.53% | 0.23% | 0.04% | ▼ Negative |

Agriculture and forest cover expanded over the study period, while surface water area declined sharply — consistent with the basin's continuing shift from semi-arid toward arid conditions. SWAT-simulated stream flow-in and flow-out varied year to year (2018–2022), tracking rainfall variability, with the lowest flows recorded in 2019 and the highest in 2018.

## Repository Contents

| File | Description |
|---|---|
| `E032_01_1516_2019 Project Report.pdf` | Full project report (dissertation) |
| `Thwake_River_Basin_Map_Atlas.png` | Composite poster of all cartographic outputs (study area, hydrogeology, rainfall, SWAT model maps, LULC change) |
| `README.md` | This file |

## Software Used

ArcGIS 10.5/10.7 · ArcSWAT · MapWindow / MWSWAT · ERDAS Imagine 2011 · ENVI · Microsoft Excel

## Recommendations

- Establish a water and climate-variability management framework for the basin.
- Improve monitoring technologies through higher-accuracy GIS models and remote sensing.
- Extend research to socio-economic and microscale hydrological modelling.
- Strengthen data availability, processing and storage practices for future assessments.

## Citation

Mwatu, M. (2023). *Assessing the Impact of Land Use and Land Cover Changes on Hydrological Processes in the Thwake River Basin Using GIS-Based Models and Remote Sensing Techniques.* BSc. Project Report, Dedan Kimathi University of Technology.
