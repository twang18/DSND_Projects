# Recommendation with IBM
### Table of Contents

1. [Installation](#installation)
2. [Project Motivation & Methodology](#motivation)
3. [File Descriptions](#files)

## Installation 
The following extra libraries are required:
- pandas, numpy, matplotlib, seaborn, sklearn, pickle
- python version: 3.6

## Project Motivation & Methodology 

Below is an example of the dashboard of IBM Watson Studio Platform.
![Platform](C:\Users\apple\Desktop\DSND Projects\4. IBM Recommendation Engine\Platform.jpg)
In this project, in order to show a recommendation board that shows the articles that are most pertinent to a specific user, I performed a study of the data available on IBM Platform, and built recommendations to particular users, using the rank of articles, user filtering and machine learning approach.

### Methodology & Procedures:
I. Exploratory Data Analysis:
- The data exploration, analysis and visualization are performed, before diving into the details fo recommendation system.
II. Rank Based Recommendations
- In order to make recommendations to new users, I first find the most popular articles based on the most interactions. 
III. User-User Based Collaborative Filtering
- In order to build better and more personalized recommendations for the users of IBM's platform, we explore users that are similar in terms of the items they have interacted with. 
IV. Matrix Factorization
- Finally, I use a machine learning approach to building recommendations called Singular Value Decomposition (SVD). Using the user-item interactions, I will build out a matrix decomposition. Using SVD, I  predict new articles an individual might interact with and thus make recommendations accordingly.
V. Conclusions & Discussions

## File Descriptions 
- Recommendations_with_IBM.ipynb: where the full code and implementations are stored
- data/articles_community.csv, data/user-item-interactions.csv
- project_tests: python file for self-test
- top_5.p, top_10.p, top_20.p: pickle files for self-tests
- user_item_matrix.p: pickle file for SVD analysis
- README.md
