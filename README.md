# Machine Learning-Based Prediction of Plane-of-Array Solar Irradiance: A Comparative Study of GTI and GHI

This repository contains the supporting code and dataset for the paper:


## 📖 Overview
Accurate prediction of solar irradiance is critical for photovoltaic (PV) systems and microgrid optimization.  
While Global Horizontal Irradiance (GHI) is commonly used, Global Tilted Irradiance (GTI) is more physically relevant for tilted PV panels but underexplored in data-driven modeling.  

This work presents a comparative analysis of GHI and GTI prediction using three machine learning regression models:
- Linear Regression (LR)  
- Decision Tree (DT)  
- Random Forest (RF)  

## 📊 Dataset
The dataset was sourced from the **Solcast API**, aggregated to hourly resolution.  
Input features include:
- Direct Normal Irradiance (DNI)  
- Diffuse Horizontal Irradiance (DHI)  
- Air temperature, relative humidity, cloud opacity, dewpoint, surface pressure, albedo, wind speed, zenith angle, etc.  

Targets:
- **Global Horizontal Irradiance (GHI)**  
- **Global Tilted Irradiance (GTI)**  

## ⚙️ Methodology
- Preprocessing: feature correlation analysis, normalization, train/validation/test split  
- Models: LR, DT, RF implemented using `scikit-learn`  
- Evaluation: R², RMSE, MAE, MSE metrics  

## 🏆 Results
- **Random Forest** achieved the best results:  
  - GTI: R² = 0.998, RMSE ≈ 12 W/m²  
  - GHI: R² = 0.9995, RMSE ≈ 6 W/m²  

This confirms the higher complexity of GTI prediction while reinforcing its relevance for PV system modeling.


