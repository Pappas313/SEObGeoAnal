# 🛰️ SatEO Analytics — Advanced Satellite Earth Observation & Geospatial Data Science

### Python | Google Colab | Sentinel-2 | Xarray | Dask | PySTAC | Rasterio | SciPy | Plotly | deck.gl

## 📖 Project Overview

**SatEO Analytics** is an advanced Python-based Earth Observation (EO) and geospatial data analytics project designed to process, analyze, and visualize satellite imagery using modern scientific computing and geospatial technologies.

The project integrates real **Sentinel-2 satellite imagery** with multidimensional data processing, parallel computing, statistical analysis, and interactive geospatial visualization.

Developed in **Google Colab**, the platform demonstrates an end-to-end satellite data analytics workflow, from satellite imagery discovery and ingestion to environmental monitoring, vegetation analysis, statistical modeling, and interactive 3D visualization.

The initial study area focuses on **Athens, Greece**, with an architecture that can be adapted to other geographic regions.

The project includes **20 scientific and geospatial visualizations**, demonstrating practical applications of Python in satellite remote sensing, environmental data science, and geographic information systems (GIS).

---

## 🎯 Project Objectives

- Discover and retrieve real Sentinel-2 satellite imagery using STAC APIs.
- Process multidimensional satellite datasets with Xarray.
- Apply parallel and lazy computation using Dask.
- Create satellite data cubes for efficient spatial and temporal analysis.
- Analyze vegetation health, water-related spectral signals, and built-up areas.
- Perform scientific calculations and statistical analysis using SciPy.
- Explore environmental changes through satellite-derived time series.
- Generate high-resolution satellite maps and statistical visualizations.
- Build interactive environmental analytics dashboards using Plotly.
- Develop interactive 3D geospatial visualizations using deck.gl and pydeck.
- Export scientific results as PNG images and interactive HTML files.

## 🛠️ Technology Stack

| Category | Technologies |
|---|---|
| Programming Language | Python |
| Development Environment | Google Colab, Jupyter Notebook |
| Satellite Data | Sentinel-2 Level-2A |
| Satellite Data Discovery | PySTAC, PySTAC Client |
| Satellite Data Provider | Microsoft Planetary Computer |
| Raster Processing | Rasterio, Rioxarray |
| Multidimensional Data | Xarray |
| Parallel Computing | Dask |
| Data Cube Processing | odc-stac |
| Data Analysis | Pandas, NumPy |
| Scientific Computing | SciPy |
| Statistical Visualization | Seaborn |
| Scientific Plotting | Matplotlib |
| Interactive Dashboards | Plotly |
| Geospatial Visualization | deck.gl, pydeck |
| Machine Learning | Scikit-learn |
| Geographic Data | GeoPandas, Shapely |

## 🏗️ System Architecture

The project follows a modular Earth Observation data-processing pipeline.

```text
             Sentinel-2 Satellite Imagery
                         |
                         v
              STAC Catalog Discovery
               PySTAC / STAC API
                         |
                         v
             Satellite Data Acquisition
           Microsoft Planetary Computer
                         |
                         v
                Raster Processing
              Rasterio / Rioxarray
                         |
                         v
                Satellite Data Cube
                Xarray / odc-stac
                         |
                         v
                Parallel Processing
                       Dask
                         |
                         v
              Spectral Index Analysis
                NDVI / NDWI / NDBI
                         |
                         v
               Scientific Analytics
            NumPy / Pandas / SciPy
                         |
              +----------+----------+
              |          |          |
              v          v          v
          Matplotlib   Plotly     deck.gl
           Seaborn    Dashboards  3D Maps
              |          |          |
              +----------+----------+
                         |
                         v
                 Export Results
                  PNG / HTML
```

## 🌍 Satellite Data Processing

### Sentinel-2 Satellite Imagery

The project uses Sentinel-2 Level-2A satellite products, providing multispectral imagery suitable for land surface monitoring and environmental analysis.

The processing pipeline uses the following spectral bands:

| Band | Description | Application |
|---|---|---|
| B02 | Blue | True-color visualization |
| B03 | Green | Water-related spectral analysis |
| B04 | Red | Vegetation analysis |
| B08 | Near Infrared | Vegetation monitoring |
| B11 | Shortwave Infrared | Built-up area analysis |
| SCL | Scene Classification | Cloud and invalid-pixel masking |

### Spectral Indices

**Normalized Difference Vegetation Index (NDVI)**

Used to assess vegetation greenness and monitor vegetation conditions.

`NDVI = (NIR - Red) / (NIR + Red)`

**Normalized Difference Water Index (NDWI)**

Used to identify surface-water-related spectral characteristics.

`NDWI = (Green - NIR) / (Green + NIR)`

**Normalized Difference Built-up Index (NDBI)**

Used to examine built-up surface characteristics.

`NDBI = (SWIR - NIR) / (SWIR + NIR)`

## 📊 Scientific & Geospatial Visualizations

The project implements 20 visualizations organized into four categories.

### 1. Satellite Imagery & Vegetation Analysis

1. **Vegetation Health Map** — Geographic visualization of NDVI values.
2. **True Color Satellite Composite** — Natural-color representation of Sentinel-2 imagery.
3. **False Color Satellite Composite** — Infrared visualization highlighting vegetation.
4. **Water Index Map** — Spatial visualization of NDWI values.
5. **Vegetation Change Detection** — Comparison of NDVI between satellite observations.

### 2. Environmental Monitoring & Time-Series Analytics

6. **Environmental Monitoring Dashboard** — Interactive NDVI, NDWI, and NDBI charts.
7. **NDVI Time-Series Analysis** — Temporal visualization of vegetation conditions.
8. **Environmental Trends Dashboard** — Comparative monitoring of spectral indices.
9. **NDVI Anomaly Heatmap** — Visualization of deviations from the study-period mean.

### 3. Statistical & Scientific Analysis

10. **Correlation Heatmap** — Relationships between satellite-derived indices.
11. **Vegetation Distribution Histogram** — Statistical distribution of NDVI pixel values.
12. **Regression Analysis** — Exploration of relationships between environmental indices.
13. **Multivariable Pair Plot** — Pairwise statistical comparisons.
14. **Environmental Box Plots** — Distribution and variability of spectral indices.
15. **Principal Component Analysis (PCA)** — Dimensionality reduction and multivariable exploration.

### 4. Interactive 3D Geospatial Visualization

16. **Interactive 3D Column Map** — Geographic columns representing NDVI intensity.
17. **3D Hexagon Density Map** — Hexagonal aggregation of geographic sample points.
18. **3D NDVI Surface** — Three-dimensional representation of vegetation-index values.
19. **Geospatial Heatmap** — Interactive spatial heatmap weighted by NDVI.
20. **Interactive 3D Scatter Plot** — Three-dimensional exploration of geographic coordinates and vegetation values.

## ⚡ Parallel Computing with Dask

Dask enables scalable processing of multidimensional satellite imagery through lazy evaluation and chunk-based computation.

Key capabilities include:

- Lazy loading of large raster datasets.
- Parallel computation across spatial and temporal dimensions.
- Reduced memory usage through chunked processing.
- Efficient calculation of spectral indices.
- Processing of satellite data cubes without loading all imagery into memory simultaneously.

## 🔬 Scientific Computing & Statistical Analysis

The project uses SciPy, Pandas, NumPy, and Scikit-learn to explore environmental datasets.

Implemented analytical techniques include:

- Descriptive statistics.
- Correlation analysis.
- Linear regression.
- Distribution analysis.
- Statistical anomaly calculations.
- Principal Component Analysis.
- Temporal aggregation.
- Satellite observation comparisons.

These techniques demonstrate how satellite-derived measurements can be transformed into interpretable environmental information.

## 🗺️ Interactive Geospatial Visualization

The project integrates **deck.gl through pydeck** to create interactive geographic visualizations.

Supported visualization layers include:

- ColumnLayer.
- HexagonLayer.
- HeatmapLayer.

Interactive features include geographic navigation, 3D visualization, color-coded environmental measurements, and hover-based data inspection.

Plotly is additionally used to generate interactive scientific charts and 3D surfaces.

## 🚀 Getting Started

### Requirements

- Google Colab or a compatible Jupyter environment.
- Python 3.
- Internet connection for satellite data access.
- Access to the Microsoft Planetary Computer public STAC API.

### Install Dependencies

```python
%pip install numpy pandas scipy xarray "dask[complete]" \
rasterio rioxarray pystac pystac-client \
planetary-computer odc-stac matplotlib seaborn \
plotly pydeck geopandas shapely scikit-learn
```

### Run the Project

1. Open the project notebook in Google Colab.
2. Install the required Python libraries.
3. Import the scientific and geospatial packages.
4. Configure the geographic bounding box and observation dates.
5. Discover Sentinel-2 imagery through the STAC API.
6. Load the imagery into an Xarray data cube.
7. Apply scene-classification-based cloud masking.
8. Calculate NDVI, NDWI, and NDBI.
9. Execute the statistical analysis and visualization cells.
10. Export the generated maps, charts, and interactive dashboards.

## 📁 Project Outputs

The project is designed to generate the following output formats:

| Output | Format |
|---|---|
| Vegetation health maps | PNG |
| Satellite RGB composites | PNG |
| Water index maps | PNG |
| Vegetation change maps | PNG |
| Statistical heatmaps | PNG |
| Regression and distribution plots | PNG |
| Interactive time-series dashboards | HTML |
| Interactive 3D geospatial maps | HTML |
| Interactive 3D scientific plots | HTML |

The exported results can be downloaded from Google Colab and incorporated into reports, scientific presentations, or other geospatial applications.

## 🌱 Potential Applications

**Environmental Monitoring:** Analyze vegetation conditions and environmental changes using satellite observations.

**Precision Agriculture:** Explore vegetation indices for agricultural monitoring and crop-health assessment.

**Urban Analytics:** Examine built-up surface characteristics and spatial land-cover patterns.

**Water Resource Monitoring:** Identify surface-water-related spectral signals and investigate changes over time.

**Climate Research:** Provide a foundation for longer-term environmental monitoring using multitemporal satellite datasets.

**Geospatial Data Science:** Demonstrate scalable processing, scientific analysis, and interactive visualization of geographic information.

## 🔮 Future Improvements

- Integrate Sentinel-1 radar imagery.
- Implement more advanced cloud and shadow detection.
- Add Copernicus DEM for true 3D terrain visualization.
- Introduce machine learning for land-cover classification.
- Develop wildfire and burn-severity monitoring.
- Implement multi-year vegetation anomaly detection.
- Add satellite imagery animations.
- Build a React-based interactive dashboard.
- Develop a Python REST API for accessing processed satellite data.
- Introduce automated satellite data ingestion and analysis pipelines.

## 🎓 Skills Demonstrated

This project demonstrates practical experience in:

- Python Software Development
- Earth Observation & Remote Sensing
- Geographic Information Systems (GIS)
- Satellite Imagery Processing
- Scientific Computing
- Multidimensional Data Analysis
- Parallel & Distributed Computing
- Statistical Analysis
- Geospatial Data Visualization
- Interactive Dashboard Development
- Data Engineering & Analytical Pipelines

## 📌 Project Summary

**SatEO Analytics** combines satellite remote sensing, scientific Python, scalable data processing, and interactive geospatial visualization into a unified Earth Observation analytics workflow.

The project demonstrates how modern Python libraries can transform raw satellite imagery into meaningful environmental indicators, statistical insights, and interactive geographic visualizations.

It serves as a practical portfolio project for **Python Developers, Data Scientists, Geospatial Software Engineers, and Earth Observation Software Engineers**.

---

**Developed with Python and Google Colab | Powered by Sentinel-2 and Open Geospatial Technologies**
