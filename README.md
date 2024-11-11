# Change Detection Analysis of Urmia Lake (2017-2024)

## 📊 Project Overview
This repository presents a comprehensive analysis of surface area changes in Urmia Lake, Iran, using Sentinel-2 satellite imagery. Urmia Lake, once one of the largest saltwater lakes in the Middle East, has experienced substantial shrinkage over the past few decades due to factors such as climate change, decreasing precipitation, and extensive human water consumption. This project aims to quantify these changes from 2017 to 2024 and analyze the impact of water management policies, especially water transfer projects.

## 🛠️ Tools and Technologies Used
- **Programming Language**: Python
- **Core Libraries**: 
  - `NumPy`, `Pandas` for data processing
  - `Matplotlib`, `Seaborn` for visualization
  - `rasterio`, `geopandas` for handling geospatial data
  - `scikit-image` for image analysis
  - `OpenCV` for computer vision techniques
- **Geospatial Tools**:
  - Google Earth Engine (GEE) for satellite data retrieval and processing
  - Sentinel-2 data for high-resolution temporal analysis

## 📂 Data Sources
This project relies on Sentinel-2 imagery accessed via Google Earth Engine. Sentinel-2 provides high-resolution multispectral data that is well-suited for detecting surface water bodies. The data was filtered to include only cloud-free images, ensuring high-quality inputs for analysis.

## 📈 Methodology

### Data Collection
- Satellite images were collected from Google Earth Engine, focusing on cloud-free scenes over the study area.
- Sentinel-2 data from 2017 to 2024 was used to capture seasonal and interannual variations.

### Data Preprocessing
- Applied atmospheric corrections to minimize distortions in raw imagery.
- Utilized the **Normalized Difference Water Index (NDWI)** to isolate water bodies from surrounding land.
- Processed data to remove noise and enhance accuracy.

### Change Detection Analysis
- Conducted time-series analysis using NDWI to track changes in the lake's surface area.
- Applied image processing techniques such as thresholding and edge detection to delineate lake boundaries.
- Quantified changes by comparing lake surface area over different time periods, particularly before and after water transfer projects.

### Visualization
- Generated graphical representations, including heatmaps and line plots, to illustrate the trend of surface area changes.
- Visualized before-and-after comparisons to highlight the effects of interventions on lake levels.

## 🚀 How to Run This Project

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/Hadikheiri/Urmia_Lake_Change_Detection.git
   cd Urmia_Lake_Change_Detection

2. **Install Required Dependencies: Make sure Python is installed, then run:**:
  ```bash
    pip install -r requirements.txt
