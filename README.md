# Predicting Soil Organic Matter Content

## Overview

This project predicts **soil organic matter content** using soil physicochemical properties and compares multiple machine learning models to identify key drivers of soil fertility.

---

## Dataset

Data sourced from Mendeley:
[https://data.mendeley.com/datasets/r7tjn68rmw/1](https://data.mendeley.com/datasets/r7tjn68rmw/1)

Includes soil measurements from Grevena, Greece such as:

* Soil texture (Sand, Silt, Clay)
* pH and Electrical Conductivity
* Macronutrients (P, K, Mg)
* Micronutrients (Fe, Zn, Mn, Cu, B)

---

## Methods

Models tested:

* Linear, Ridge, Lasso, Elastic Net
* Polynomial Regression
* KNN
* Random Forest
* Boosted Trees (XGBoost)

Workflow:

* Train/test split (75/25)
* 5-fold cross-validation
* Feature scaling + preprocessing via `tidymodels`

---

## Results

Best model: **Boosted Trees**

* Lowest RMSE (~0.47–0.48)
* Random Forest close second (~0.47)
* Linear models performed slightly worse

---

## Key Insights

* **Potassium (K)** is the strongest predictor of organic matter
* Sand content negatively impacts soil quality
* Tree-based models outperform linear models
* Soil composition strongly influences fertility

---

## Tools

`tidymodels`, `xgboost`, `ranger`, `ggplot2`, `corrplot`

---

## Goal

Use machine learning to better understand soil health and improve agricultural decision-making.
