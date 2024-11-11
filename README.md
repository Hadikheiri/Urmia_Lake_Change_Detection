Change Detection Analysis of Urmia Lake (2017-2024)
📊 Project Overview
This repository presents a comprehensive analysis of surface area changes in Urmia Lake, Iran, using Sentinel-2 satellite imagery. Urmia Lake, once one of the largest saltwater lakes in the Middle East, has experienced substantial shrinkage over the past few decades due to factors such as climate change, decreasing precipitation, and extensive human water consumption. The aim of this project is to quantify these changes from 2017 to 2024 and analyze the impact of water management policies, especially water transfer projects.

🛠️ Tools and Technologies Used
Programming Language: Python
Core Libraries:
NumPy, Pandas for data processing
Matplotlib, Seaborn for visualization
rasterio, geopandas for handling geospatial data
scikit-image for image analysis
OpenCV for computer vision techniques
Geospatial Tools:
Google Earth Engine (GEE) for satellite data retrieval and processing
Sentinel-2 data for high-resolution temporal analysis
📂 Data Sources
This project relies on Sentinel-2 imagery accessed via Google Earth Engine. Sentinel-2 provides high-resolution multispectral data that is well-suited for detecting surface water bodies. The data was filtered to include only cloud-free images, ensuring high-quality inputs for analysis.

📈 Methodology
Data Collection:

Satellite images were collected from Google Earth Engine focusing on cloud-free scenes over the study area.
Sentinel-2 data from 2017 to 2024 was used to capture seasonal and interannual variations.
Data Preprocessing:

Applied atmospheric corrections to minimize distortions in raw imagery.
Utilized the Normalized Difference Water Index (NDWI) to isolate water bodies from surrounding land.
Processed data to remove noise and enhance accuracy.
Change Detection Analysis:

Conducted time-series analysis using NDWI to track changes in the lake's surface area.
Applied image processing techniques such as thresholding and edge detection to delineate lake boundaries.
Quantified changes by comparing lake surface area over different time periods, particularly before and after water transfer projects.
Visualization:

Generated graphical representations, including heatmaps and line plots, to illustrate the trend of surface area changes.
Visualized before-and-after comparisons to highlight the effects of interventions on lake levels.
🚀 How to Run This Project
Follow these steps to replicate the analysis on your local system:

Clone the Repository:

bash
Copy code
git clone https://github.com/yourusername/UrmiaLake_ChangeDetection.git
cd UrmiaLake_ChangeDetection
Install Required Dependencies: Make sure Python is installed, then run:

bash
Copy code
pip install -r requirements.txt
Authenticate Google Earth Engine: Set up a Google Earth Engine account and authenticate your environment:

python
Copy code
import ee
ee.Authenticate()
ee.Initialize()
Execute the Analysis: Run the main analysis script:

bash
Copy code
python main.py
Access the Results: Results, including visualizations and metrics, will be saved in the output/ directory.

📊 Results and Insights
The analysis reveals a significant reduction in Urmia Lake's surface area over the study period, highlighting the impact of environmental and anthropogenic factors. The NDWI-based analysis clearly indicates how the lake's extent has diminished, especially following the implementation of water management projects. Key findings include:

Yearly changes in lake surface area.
Visual evidence of surface area reduction through satellite image analysis.
Correlations between water management interventions and lake recovery.
🌍 Future Directions
Integrating Machine Learning: Future work could involve the use of machine learning models to improve the accuracy of water body classification and predict future changes.
Expanding Analysis Scope: Additional variables such as temperature, precipitation, and groundwater extraction data can be incorporated to enrich the analysis.
Automating Data Updates: Setting up automated pipelines to periodically analyze new satellite data could provide ongoing insights.
🤝 Contributing
Contributions to this project are welcome. Feel free to submit a pull request or open an issue for suggestions and improvements.
