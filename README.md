# AMES IA Housing Data - EDA and Modeling


![LinReg Results](data/assets/Linreg_rsults.PNG)



## Overview and Current Status
- EDA, feature selection, and modeling of the AMES IA housing dataset
- Model parameters can be further optimized
- More work can be done including location-based features

### Workflow
1. EDA - loads the Housing data, cleans and investigates the data, and selects features for Modeling
2. Modeling - instantiates and runs and Linear Model and a DNNRegressor using the Tensorflows API

### Problem Statement
- What are the key drivers of housing prices?
- Can we build a generalized model that is able to make sense of qualitative and quantitave features?


## DATA

### Ames IA Housing Dataset
- Data located here: https://www.kaggle.com/c/house-prices-advanced-regression-techniques/data
- Data Documentation located here: (http://jse.amstat.org/v19n3/decock/DataDocumentation.txt)


## EDA and Feature Selection

- Potential features were identified by filling missing values, investigating distributions, and checking relationships between each feature and the target variable - SalePrice.
- Categorical Variables were grouped by sale price, and encoded as numeric, to allow for more flexibility in modeling
- Features were selected based on their relative strength in prediciting the target variable, and for their intuitive interpretatiblity, striking a balance between overfitting the model and model performance


![Qualitative Features](data/assets/qual_features.PNG)


## Modeling

- Two Models were fit on the training data
    - A Linear Regression Model - RMSE: 0.14827
    - A DNNRegressor using the Tensorflows Esitmator API
    


### Conclusions

Features to consider - garage quality, basement condition, living area, all significantly positively correlated with Housing Price

Neighborhoods to watch - Stonebridge and Northbridge Heights have the highest housing pricesan and square footage

### Further Study

Create neighborhood buckets and find stronger relationship between location and price