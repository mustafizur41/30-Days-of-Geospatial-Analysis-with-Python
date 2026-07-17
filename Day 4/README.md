This project demonstrates how to create a **publication-quality soil texture map of France** by integrating **Google Earth Engine (GEE)** for raster processing and **Python** for geospatial visualization and cartographic design.

The workflow combines cloud-based geospatial processing with Python's powerful GIS ecosystem to produce a clean, high-resolution thematic soil texture map based on the **USDA Soil Texture Classification System**.

---

## 📌 Project Overview

The analysis consists of two main parts:
- **Google Earth Engine (GEE):** Processing and exporting the soil texture raster.
- **Python:** Loading, clipping, classifying, and visualizing the exported raster using GeoPandas, Rasterio, and Matplotlib.

---

## 🗂 Workflow

### 1. Administrative Boundary Preparation (Python)
- Download France administrative boundaries (ADM0 and ADM1) from **geoBoundaries**
- Visualize country and regional boundaries
- Export the country boundary as a shapefile for Google Earth Engine

---

### 2. Google Earth Engine Processing
Inside Google Earth Engine:
- Import the France boundary
- Load the OpenLandMap Soil Texture dataset
- Clip the raster using the France boundary
- Export the **b0** soil texture band as a GeoTIFF

---

### 3. Raster Processing (Python)
- Load the exported GeoTIFF
- Reproject the raster to match the CRS of the administrative boundary
- Clip the raster to France's national boundary

---

### 4. Soil Texture Classification
Convert the raster values into USDA soil texture classes.
The following classes are included:
- Clay
- Silty Clay
- Sandy Clay
- Clay Loam
- Silty Clay Loam
- Sandy Clay Loam
- Loam
- Silty Loam
- Sandy Loam
- Silt
- Loamy Sand
- Sand

Each class is assigned a custom color palette for visualization.

---

### 5. Cartographic Visualization
The final map includes:
- Soil texture raster
- France national boundary (ADM0)
- Regional boundaries (ADM1)
- Customized soil texture legend
- Map title and subtitle
- Source and author information
- High-resolution PNG export (300 dpi)

---

## 📊 Data Sources

### Administrative Boundaries

**geoBoundaries**
https://www.geoboundaries.org/

GitHub Repository:
https://github.com/wmgeolab/geoBoundaries

---

### Soil Texture Dataset

**OpenLandMap**
OpenLandMap Soil Texture Class (USDA System)

Dataset:
https://developers.google.com/earth-engine/datasets/catalog/OpenLandMap_SOL_SOL_TEXTURE-CLASS_USDA-TT_M_v02

## 📈 Output

The final output is a publication-quality thematic map showing the spatial distribution of USDA soil texture classes across France.

Features include:
- Administrative boundaries
- Soil texture classification
- Custom legend
- High-resolution export
- Ready for reports, presentations, or publications

---

## 🎯 Learning Objectives

This project demonstrates how to:
- Work with vector and raster geospatial datasets
- Integrate Google Earth Engine with Python
- Reproject and clip raster data
- Apply categorical color mapping
- Design publication-quality thematic maps
- Build reproducible geospatial workflows

---

## 📄 License

This project is intended for educational and research purposes.

Please cite the original data providers when using the datasets in academic work.
