# Wildfire Prediction using Geospatial Analysis

This project aims to develop a predictive model for wildfire occurrences in California using climate and geospatial data. By leveraging climate data and geospatial features, the model provides insights into wildfire risks, enhancing disaster management and informing public safety strategies.

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Project Structure](#project-structure)
- [Technologies Used](#technologies-used)
- [Data Sources](#data-sources)
- [Modeling Approach](#modeling-approach)
- [Results](#results)
- [Contributors](#contributors)

## Overview
Wildfires in California pose a growing threat due to climate change and increasing urban expansion. This project utilizes geospatial and temporal climate data to predict wildfire occurrences across California, enabling proactive resource allocation, public safety measures, and improved disaster readiness.

## Features
- **Climate Data Analysis**: Examines temperature and rainfall as primary climate variables influencing wildfire occurrences.
- **Geospatial Processing**: Uses CAL FIRE perimeter data to analyze wildfire-prone regions.
- **Time Series Analysis**: Extracts time series features to identify seasonal patterns in fire events.
- **Predictive Modeling**: Employs machine learning models to predict the likelihood of wildfire events.

## Project Structure

wildfire-prediction/ ├── data/ │ ├── climate_data.csv │ ├── fire_perimeter_data.gdb ├── notebooks/ │ ├── data_preprocessing.ipynb │ ├── modeling.ipynb ├── reports/ │ └── Capstone_Report.pdf ├── README.md └── requirements.txt


- **data/**: Contains the climate and fire perimeter datasets.
- **notebooks/**: Jupyter notebooks for data processing and model development.
- **reports/**: Project report summarizing findings and methodologies.
- **README.md**: Overview of the project and usage instructions.
- **requirements.txt**: List of dependencies for the project.

## Technologies Used
- **Python**: Core programming language for data analysis and modeling.
- **Machine Learning Libraries**: Includes Random Forest, XGBoost, LightGBM, and AdaBoost.
- **Geospatial Tools**: Utilizes GIS software and libraries (e.g., `geopandas`) for spatial data processing.
- **Data Visualization**: Uses `matplotlib` and `seaborn` for visualizations.


## Data Sources
- **Climate Data**: Collected from the PRISM Climate Group, includes monthly temperature and rainfall data.
- **Fire Perimeter Data**: Sourced from CAL FIRE, provides historical wildfire perimeters in California.

## Modeling Approach
1. **Data Preprocessing**: Climate data is processed to extract time series features, including mean, median, max, and min temperatures and precipitation.
2. **Principal Component Analysis (PCA)**: Used to visualize clusters and patterns in fire and no-fire events.
3. **Model Training**:
   - Trained multiple machine learning models including Random Forest, XGBoost, LightGBM, and AdaBoost.
   - Models were evaluated on recall and precision metrics, prioritizing recall for fire events.
4. **Hyperparameter Tuning**: Utilized GridSearchCV to optimize model parameters.

## Results
- **Best Model**: Random Forest showed the highest recall for predicting fire events, essential for minimizing missed detections.
- **Accuracy**: Random Forest achieved an accuracy of ~90%, with optimal settings for `n_estimators` and `max_depth`.
- **Challenges**: High false positives in some models indicate a need for balancing precision without sacrificing recall.

## Contributors
- Sai Narayana Murthy Dontukurti
- Sasank Reddy Chaganti

Thank you for reviewing the **Wildfire Prediction using Geospatial Analysis** project!
