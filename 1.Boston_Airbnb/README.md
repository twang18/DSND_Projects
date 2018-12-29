# Boston Airbnb Data Exploration & Price Prediction

### Table of Contents

1. [Installation](https://github.com/twang18/1.Boston_Airbnb#installation)
2. [Project Motivation](https://github.com/twang18/1.Boston_Airbnb#motivation)
3. [File Descriptions](https://github.com/twang18/1.Boston_Airbnb#files)
4. [Results](https://github.com/twang18/1.Boston_Airbnb#results)

## Installation

The following extra libraries are required.

- pandas, numpy, matplotlib, seaborn, sklearn
- python version: 3.6

## Project Motivation

The data sets of Airbnb describing the the listing activity of homestays in Boston, MA, are both available on [Kaggle](https://www.kaggle.com/airbnb/boston) and [Airbnb Websites](http://insideairbnb.com/get-the-data.html).

I am particularly interested in the following three questions:

1. What are the busiest times of the year to visit Boston? Do prices spike and vacancy drop during that period?
2. Are there any price differences among different neighborhoods? Which neighborhoods are the most popular?
3. Other than all the reviews and descriptions, what other features affect the listing price? Is there a model to predict the listing prices?

## File Descriptions

- Boston Airbnb Data Analysis.ipynb: A Jupyter Notebook with detailed codes and descriptions
- Three Tips for Airbnb users to Boston.pdf: the blog post of the data analysis and findings
- Datasets: listings.csv, calendar.csv
- README.md

## Results

### Methodology

- Data wrangling (handling with NaN, outliers, undesired data types, etc.)
- EDA & visualization
- Model regression & price prediction

### Results

- September is the busiest time in Boston, with Airbnb vacancy rate drops drastically and average listing prices increases by 20%.
- Leather District has the highest average listing price, followed by the neighborhoods of South Boston Waterfront and Bay Village.
- Model regression for price prediction with respect to property-related features was carried out; Feature selection was conducted; both Ridge model and Gradient Boosting model were used together with Grid Search. A model with a R2 score of 0.656 was obtained.
- A Blog on the non-technical findings of Boston Airbnb data sets are available [here](https://github.com/twang18/blog/blob/master/Three%20Tips%20for%20Airbnb%20users%20to%20Boston.pdf).