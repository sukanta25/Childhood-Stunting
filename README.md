
# Childhood Stunting in Bangladesh

## Integrating Environmental Data, Spatial Epidemiology, and Machine Learning to Characterize Childhood Stunting in Bangladesh

### Overview
This research investigates childhood stunting in Bangladesh by integrating national survey data, environmental indicators, spatial epidemiology and machine learning.

### Data Sources
- Bangladesh Demographic and Health Survey (BDHS 2022)
- Google Earth Engine
- MODIS
- ERA5-Land
- CHIRPS
- SRTM
- WorldPop
- TerraClimate

### Methodology

**1. Data Integration**
- Integrated BDHS 2022 survey records with geographic coordinates and environmental indicators.
- Analyzed 3,633 children from 667 geographic clusters.
- Used 3,620 complete-case observations for machine learning.

**2. Spatial Analysis**
- Global Moran's I
- Local Moran's I (LISA)
- Getis-Ord Gi*
- Geographically Weighted Regression (GWR)
- Multiscale Geographically Weighted Regression (MGWR)

**3. Machine Learning**
- Gradient Boosting-based feature selection
- Recursive Feature Elimination with Cross-Validation (RFECV)
- Sequential Backward Feature Selection
- Evaluation of 13 machine learning classifiers
- Survey-weighted modeling and PSU-disjoint validation

**4. Explainable AI**
- GeoShapley for geographic and feature-level interpretation

### Key Findings
- Survey-weighted childhood stunting prevalence: 22.84%.
- Spatial clustering was generally weak and sensitive to neighborhood definitions.
- MGWR achieved an in-sample R² of 0.1884.
- The grouped backward feature selection and AdaBoost pipeline achieved a held-out comparative ROC-AUC of 0.6773.
- Further independent validation is needed before operational use.

### Repository Contents
- `Gradient Boosting.ipynb`
- `RFECV final.ipynb`
- `Sequential Backward.ipynb`
- `Spatial Final(Stunting).ipynb`

### Research Team
- Sukanta Das
- Md. Mahamudul Islam
- Suman Biswas

Department of Statistics and Data Science  
Islamic University, Kushtia, Bangladesh

### Data Availability
BDHS data are subject to DHS Program access conditions. Restricted individual-level survey data are not distributed through this repository.
