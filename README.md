# Machine Learning–Based Estimation of NO₂ and O₃ over Germany

This repository contains the code associated with the published work:

> **Balamurugan, V., Chen, J., Wenzel, A., and Keutsch, F. N.**  
> *Spatio-temporal modeling of air pollutant concentrations in Germany using machine learning*  
> **Atmospheric Chemistry and Physics**, 2023  
> https://doi.org/10.5194/acp-23-10267-2023

The study presents a machine learning framework for estimating near-surface **NO₂** and **O₃** concentrations over Germany by integrating satellite observations, meteorological variables, land-use information, and emission-related predictors, with emphasis on robust spatial and temporal validation.

---

## Repository Contents

This repository provides:

- End-to-end machine learning workflows for NO₂ and O₃ prediction
- Model development using **XGBoost** and **neural network (MLP)** regressors
- Multiple validation strategies:
  - Random cross-validation
  - Time-based (leave-time-out) cross-validation
  - Spatial (leave-location-out) cross-validation
- Model interpretability using **SHAP (SHapley Additive exPlanations)**
- Publication-quality visualizations

---

## Data Availability and Reproducibility

Due to data size constraints, **raw observational and satellite datasets are not publicly redistributed in this repository**.

📩 **To request the preprocessed data**, please contact the corresponding author as indicated in the publication.

---

## Methodology Overview

The modeling framework integrates:

- **Satellite observations** (e.g., TROPOMI NO<sub>2</sub>, O<sub>3</sub> and HCHO)
- **Meteorological variables** (boundary layer height, wind speed/direction, temperature, humidity)
- **Land-use and vegetation indices** (NDVI)
- **Emission and proxy variables (road density)**
