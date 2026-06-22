# Philippine Mountains Dataset 🇵🇭⛰️

A cleaned and enriched dataset of Philippine mountains and peaks for geospatial analysis, data visualization, and outdoor exploration.

---

## Project Overview

The goal of this project is to create a BI-ready Philippine mountains dataset that can be used for:

* interactive maps
* Tableau / Power BI dashboards
* regional mountain analysis
* elevation and prominence insights
* hiking and summit exploration tools

This dataset is part of my data analytics portfolio project focused on geospatial data cleaning, enrichment, and visualization.

---

## Dataset Contents

The final dataset includes mountain-level information such as:

| Column               | Description                                                  |
| -------------------- | ------------------------------------------------------------ |
| `mountain_id`        | Unique identifier for each mountain                          |
| `name`               | Standardized mountain name                                   |
| `elev`               | Elevation in meters                                          |
| `prom`               | Prominence in meters, if available                           |
| `lat`                | Latitude                                                     |
| `lon`                | Longitude                                                    |
| `coord`              | Coordinate pair                                              |
| `is_volc`            | Indicates whether the mountain is volcanic                   |
| `prov`               | Assigned Philippine province                                 |
| `region`             | Assigned Philippine region                                   |
| `isl_grp`            | Island group: Luzon, Visayas, or Mindanao                    |
| `source`             | Original data source                                         |
| `data_quality_notes` | Notes about validation, missing values, or enrichment status |

---

## Data Cleaning Process

The data pipeline includes:

1. **Name standardization**
   Cleaned mountain names for consistent matching and deduplication.

2. **Coordinate validation**
   Checked latitude and longitude values and flagged invalid or uncertain coordinates.

3. **Administrative assignment**
   Used geospatial boundaries to assign each mountain to its province, region, and island group.

4. **Duplicate handling**
   Deduplicated records by mountain name and location while preserving useful source information.

5. **Elevation, Prominence and Volcanic enrichment**
   Filled missing elevation values where possible using external mountain pages.

6. **BI-ready export**
   Organized the final columns and prepared the dataset for Tableau, Power BI, and mapping tools.

---

## Visualization

An interactive dashboard is being built to explore Philippine mountains by:

* island group
* region
* elevation
* volcanic classification
* hiking difficulty/personality match
* top mountain recommendations

Dashboard link: Coming soon

---

## Current Status

* [x] Collected Philippine mountain data from public sources
* [x] Cleaned and standardized mountain names
* [x] Assigned province, region, and island group
* [x] Enriched priority mountains with elevation/prominence/volcanic status data
* [x] Finalize missing elevation enrichment
* [x] Export final CSV and GeoJSON
* [ ] Publish Tableau dashboard
* [ ] Publish Power BI dashboard

---

## Data Limitations

This dataset is still being improved. Some records may have:

* missing elevation or prominence values
* inconsistent names across sources
* approximate coordinates
* duplicate or near-duplicate mountain entries
* limited information for lesser-known peaks

Each record includes source and quality notes where available.

---

## Tools Used

* Python
* Pandas
* GeoPandas
* BeautifulSoup
* Requests
* OpenStreetMap / Overpass
* Tableau
* GitHub

---
## Data Sources

This dataset was compiled and validated using multiple public sources, including:

* OpenStreetMap / Overpass data for named Philippine peaks
* GeoNames / QuickTools mountain records
* PeakVisor pages for selected elevation, prominence and volcanic classification enrichment
* Philippine administrative boundary files for province and region assignment through spatial validation
* Github repository / phl - mountains for elevation, prominence and volcanic classification enrichment
  
Because mountain data can vary across sources, this project keeps source tracking and quality notes to make the dataset more transparent.

### Source Links

- OpenStreetMap: https://www.openstreetmap.org/
- PeakVisor: https://peakvisor.com/
- phl-mountains: https://github.com/j4ckofalltrades/phl-mountains
- Philippines JSON Maps: https://github.com/faeldon/philippines-json-maps


## License

This project is shared for educational and portfolio purposes.

Please check the original data source licenses before using this dataset commercially.

---

Data Analytics / BI / Geospatial Portfolio Project
