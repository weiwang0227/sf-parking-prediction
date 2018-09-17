# Overview
By leveraging [Scikit-learn](http://scikit-learn.org/)'s machine learning technology, this project is for practicing the prediction to se if at least one parking spot is available at a specified street segment and at a given time in San Francisco. This is a project for Kaggle challenge [Parking in SF](https://www.kaggle.com/c/parking-in-sf/). 
The result is a little bit above the average among the participants in this competition.

# Techniques
Multiple techniques are leveraged to do the feature engineering and predictions
* Unify the street segments by creating "block id" according to the starting and ending intersection latitude & longitude 
* Generate extra date-relevant features, such as day-of-week, is_holiday
* Merge multiple features scattering in separate data frames (or data tables)
* Convert features whose type is string into numeric for fitting Random Forest Classifier
* Mean encoding for filling NA (not available) features
* Leverage Grid Search to find the best fitting for Random Forest Classifier by measuring fbeta score

# Tools and packages
* pandas
* numpy
* scikit-learn
* geopy
* geocoder

# Data
The raw data can be downloaded at [here](https://www.kaggle.com/c/parking-in-sf/data)

