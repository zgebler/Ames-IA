# Project 2 - Ames Housing Data and Kaggle Challenge



## Question

What are the factors that drive housing prices? How can we build a model that will predict the price of a house?


## DATA

data dictionary located here: (http://jse.amstat.org/v19n3/decock/DataDocumentation.txt)


Training data set: 2037 rows X 81 columns

Missing Values - Formatting conditions. no significant errors in data

Outliers - per data dictionary, removed houses with living area > 4000 sq ft and Sale Price > $500_000


## Feature Selection and Modeling

Based on correlations in training data, selected features that would give significant effects on sale price

included locational dummies based on neighborhood

Used a LinearRegression model, fit on the training data and then made predictions on the test dataset


### Conclusions

Features to consider - garage quality, basement condition, living area, all significantly positively correlated with Housing Price

Neighborhoods to watch - Stonebridge and Northbridge Heights have the highest housing pricesan and square footage

### Further Study

Create neighborhood buckets and find stronger relationship between location and price