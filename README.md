# Exploratory analysis for the Boston Airbnb listings

This repository contains code and data supporting the verbose presentation posted [here](https://cmageanu.github.io/abnb_boston)

Original location of data is at [Kaggle]((https://www.kaggle.com/airbnb/boston)

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