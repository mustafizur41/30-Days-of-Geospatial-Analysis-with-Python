# 🌍 Bivariate Climate Mapping with TerraClimate Data in Python

> **Inspiration:** This project was inspired by the outstanding work and visualization concepts from: Milan Janosov (https://milanjanosov.substack.com/p/bivariate-climate-map-temperature?triedRedirect=true)

**Official TerraClimate Website:**  
https://www.climatologylab.org/terraclimate.html

---

## 📖 Project Overview

This project demonstrates how to build a **bivariate climate map** by combining **annual maximum temperature (Tmax)** and **annual precipitation (PPT)** from the **TerraClimate** dataset using Python.

Unlike traditional single-variable maps, a bivariate map allows two environmental variables to be visualized simultaneously, making it easier to identify climate patterns such as:

- 🔥 Hot & Dry
- 🌧 Cold & Wet
- 🔥 Wet & Hot
- ❄ Cold & Dry

The workflow includes downloading climate raster data, clipping it to a selected study region, smoothing raster values, classifying both climate variables into quantiles, generating a custom 4×4 bivariate color palette, and producing a publication-quality map with an embedded legend.

---

## ✨ Features

- Load TerraClimate NetCDF climate datasets
- Read Natural Earth country boundaries
- Select a continent, country, or the entire world
- Clip raster datasets to any region
- Apply Gaussian smoothing to reduce raster noise
- Quantile classification for temperature and precipitation
- Create a custom 4×4 bivariate color palette
- Generate a bivariate climate classification raster
- Automatically build a two-dimensional legend
- Export high-resolution (300 DPI) publication-ready maps

---

## 📊 Data Sources

### TerraClimate

TerraClimate is a high-resolution (~4 km) monthly global climate dataset that combines climate normals with time-varying meteorological observations.

Variables used in this project:
- Annual Maximum Temperature (Tmax)
- Annual Precipitation (PPT)

---

### Natural Earth

Country boundary data comes from the Natural Earth dataset.
https://www.naturalearthdata.com/

---

## 🛠 Python Libraries

- GeoPandas
- Rasterio
- Rioxarray
- Xarray
- NumPy
- SciPy
- Matplotlib
- Shapely

---

## 🌡 Climate Variables

### Temperature

Annual Maximum Temperature (Tmax)

### Precipitation

Annual Total Precipitation (PPT)

---

## 📈 Example Output

The final map includes:
- Bivariate climate raster
- Country boundaries
- Embedded two-dimensional legend
- Publication-quality layout
- Automatic export as PNG

---

## 🎯 Applications
This workflow can be adapted for numerous environmental and climate studies, including:
- Climate change analysis
- Agricultural suitability mapping
- Drought assessment
- Ecological zoning
- Biodiversity research
- Environmental monitoring
- Regional climate comparison
- Land suitability assessment

---

## 📜 License

This repository is intended for educational and research purposes.

Please review the TerraClimate data usage and citation guidelines before using the dataset in publications or commercial applications.
