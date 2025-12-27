# San Francisco Crime Geodata Analysis & Prediction

This repository provides an end-to-end analytical pipeline for exploring, visualizing, and predicting crime patterns in San Francisco using historical data (July - Dec 2012). The project employs advanced geospatial processing, time-series forecasting, and machine learning to uncover insights into urban safety.

## 🚀 Key Features

- **Modular Data Pipeline**: Automated ingestion and consolidation of disparate crime category shapefiles (Robbery, Vandalism, Car Theft, Drugs).
- **Advanced Preprocessing**: Robust temporal normalization and feature engineering, resolving critical data quality issues like time-parsing errors.
- **Predictive Analytics**:
    - **Time-Series Forecasting**: Implements **ARIMA** models to predict daily crime volumes.
    - **Incident Classification**: Uses **Random Forest** to classify incident resolutions (e.g., predicting arrests) based on spatial and temporal features.
- **Geospatial Intelligence**: Layering crime incidents with census block demographics for urban spatial analysis.
- **Interactive Visualizations**: includes animated heatmaps and district-level distribution plots.

## 🛠️ Technology Stack

- **Data Manipulation**: `pandas`, `numpy`
- **Geospatial Analysis**: `geopandas`, `shapely`, `fiona`
- **Modeling**: `scikit-learn`, `statsmodels` (ARIMA)
- **Visualization**: `seaborn`, `matplotlib`, `wordcloud`

## 📁 Project Structure

- `Advanced Analytics.ipynb`: The primary analytical notebook, structured as a professional logical report.
- `SFCrime_July_Dec2012 2/`: Core data directory containing:
    - `Crime Events/`: Raw ESRI Shapefiles.
    - `SF PD Plots/`: Geospatial boundaries and census block data.
- `cleaned_crime_data.*`: Processed geospatial dataset ready for GIS applications.
- `sf_crime_animated_heatmap.html`: Interactive temporal visualization of crime density.

## 📊 Analytical Workflow

1.  **Environment Configuration**: initializing libraries and global visualization settings.
2.  **Modular Ingestion**: Consolidation of categorical geospatial data.
3.  **Refinement & Feature Engineering**: Standardizing formats and extracting temporal dimensions (Hour, DayOfYear, Month).
4.  **Descriptive Profile**: Statistical analysis of incident distributions across SF Districts.
5.  **Predictive Modeling**: Application of ARIMA for volume forecasting and Random Forest for behavioral classification.
6.  **Spatial Overlay**: Merging crime data with demographic census layers.
7.  **Systematic Export**: saving refined artifacts for downstream BI consumption.

## 💾 Installation & Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/AveryDoan/Geodata-Analysis-SanFrancisco-Crime-Incident.git
   ```
2. Install dependencies:
   ```bash
   pip install geopandas pandas shapely statsmodels scikit-learn seaborn matplotlib wordcloud
   ```
3. Open `Advanced Analytics.ipynb` in your preferred Jupyter environment and run Phase 1 through Phase 7.

---
**Author**: Avery Doan
**Data Source**: San Francisco Open Data Portal