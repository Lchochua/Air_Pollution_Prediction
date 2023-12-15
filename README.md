# Air Pollution Prediction

Air pollution, notably PM2.5, an airborne pollutant of microscopic dimensions, presents a significant hazard to human health and environmental well-being. These minute particles, with a diameter less than 2.5 micrometers, possess the capacity to infiltrate deeply into the respiratory system, leading to a spectrum of health issues, including respiratory infections, cardiovascular ailments, and premature mortality.

Conventional PM2.5 monitoring has traditionally relied on ground-based sensors; however, their restricted coverage and substantial expenses have constrained comprehensive global surveillance efforts. In response to this challenge, a cost-effective ML-based solution is offered to predict PM2.5 levels for different geographic areas.

## Methodology

The implimentation starts with an Exploratory Data Analysis (EDA) phase aimed at comprehensively examining the dataset. Subsequently, a range of regression techniques is employed, including simple linear regression, Ridge regression, and Lasso regression. Additionally, Random Forest and Extra Trees methods are subject to scrutiny.

Nevertheless, it is evident that the utilization of individual models fails to produce satisfactory results. In response to this, the adoption of ensemble methods, specifically a stacking model, is implemented. This strategy combines the capabilities of multiple models to formulate a more robust and precise predictive model.

Concurrently, and in parallel with the modeling exercise, a detailed error analysis is conducted. Furthermore, a series of rigorous validation exercises are performed to ascertain the dependability and effectiveness of the final predictive model.

## Dataset
​
In the project Ground Based-Sensors in train data used as target and model trained with 5P Satellite Data and The Global Forecast System (GFS) data.
​
The Zindi Channel and Dataset: [Urban Air Pollution Challenge](https://zindi.africa/competitions/urban-air-pollution-challenge).
​
### Features
​
- [Weather Data](https://developers.google.com/earth-engine/datasets/catalog/NOAA_GFS0P25).
- [NO2: Offline Nitrogen Dioxide](https://developers.google.com/earth-engine/datasets/catalog/COPERNICUS_S5P_OFFL_L3_NO2).
- [AER AI: Offline UV Aerosol Index](https://developers.google.com/earth-engine/datasets/catalog/COPERNICUS_S5P_OFFL_L3_AER_AI).
- [SO2: Offline Sulfur Dioxide](https://developers.google.com/earth-engine/datasets/catalog/COPERNICUS_S5P_OFFL_L3_SO2).
- [CH4: Offline Methane](https://developers.google.com/earth-engine/datasets/catalog/COPERNICUS_S5P_OFFL_L3_CH4).
- [O3: Offline Ozone](https://developers.google.com/earth-engine/datasets/catalog/COPERNICUS_S5P_OFFL_L3_O3).
- [CO: Offline Carbon Monoxide](https://developers.google.com/earth-engine/datasets/catalog/COPERNICUS_S5P_OFFL_L3_CO).
- [HCHO: Offline Formaldehyde](https://developers.google.com/earth-engine/datasets/catalog/COPERNICUS_S5P_OFFL_L3_HCHO).
- [CLOUD: Near Real-Time Cloud](https://developers.google.com/earth-engine/datasets/catalog/COPERNICUS_S5P_OFFL_L3_CLOUD).
​
​

## Requirements and Environment
​
Requirements:
- pyenv with Python: 3.11.3

​
Environment: 
​
```Bash
pyenv local 3.11.3
python -m venv .venv
source .venv/bin/activate
pip install --upgrade pip
pip install -r requirements.txt
```
​