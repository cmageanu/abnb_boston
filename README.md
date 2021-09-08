# Exploratory analysis for the Boston Airbnb listings

This repository contains code and data supporting the verbose presentation posted [here](https://cmageanu.github.io/abnb_boston)

Original location of data is at [Kaggle]((https://www.kaggle.com/airbnb/boston)

## Motivation for this project

This project is part of an assignment of the [Udacity Data Science nano degree program](https://www.udacity.com/course/data-scientist-nanodegree--nd025)

The main motivation is of course to successfully complete the assignment but in doing so, I tried to put in practice the knowledge acquired on the course above, specifically the [CRISP-DM](https://en.wikipedia.org/wiki/Cross-industry_standard_process_for_data_mining) approach.

Overall the code in this repository aims to answer the following three questions:

1. Are there interesting features in the data set which support the common expectation of an Airbnb user? Can we spot interesting facts by looking just how such features are correlated?
2. Can we predict prices better than the simple average value of $174?
3. What are the most important features determining the price of a listing?

## Files
### Data files

listings.csv - main subject of the analysis; it contains prices and features for the Airbnb listings in the Boston area
reviews.csv - contains text reviews for the Boston Airbnb listings
calendar.csv - contains a list of (listing_id, date, availablity, price) items, again in the context of Boston Airbnb area
Inside Airbnb Data Dictionary - listings.csv detail v4.csv --- name self descriptive

### Modules required to run the code

numpy
pandas
sklearn
xgboost
matplotlib
seaborn

The code was tested in a conda created environment using conda 4.10.3 with Python 3.7.7 running on Ubuntu 20.04

### Code

Airbnb_Boston.ipynb

The code explores the listings.csv data set.

The goal is to look at how the features influence the price column in the listings data set.

There are a few steps for preparing the data - mostly addressing missing values and categorical features.

A correlation matrix for the numeric features is produced.

Finally, 3 sets of predicting algorithms are tried. Feature importance is presented.

## Summary of the analysis

1. We find clusters of correlated features and attempt to explain why the correlations occur.
2. We run 3 predictive algorithms and find improvements on the coarse price estimation made by averaging the price of all listings.
3. We extract the top features ranked by their importance in two of our models and comment on the significance of the findings.