# Disaster Response Pipeline Project

### Table of Contents

1. [Installation](https://github.com/twang18/3.Disaster_Response_Pipeline#installation)
2. [Project Motivation & Methodology](https://github.com/twang18/3.Disaster_Response_Pipeline#motivation)
3. [File Descriptions](https://github.com/twang18/3.Disaster_Response_Pipeline#files)
4. [Results](https://github.com/twang18/3.Disaster_Response_Pipeline#results)

## Installation

The following extra libraries are required:

- pandas, numpy, matplotlib, seaborn, sklearn, json, plotly, nltk, sqlalchemy
- python version: 3.6

## Project Motivation & Methodology

In this project, I applied data engineering skills to analyze disaster data from Figure Eight to build a model for an API that classifies disaster messages. The major procedure is as follows:

1. Data ETL: I conduct the Extract, Transform, and Load process to Figure Eight real messages; read the dataset; clean the data, and then store it in a SQLite database.
2. Machine Learning pipeline: I apply a machine learning pipeline together with NLP technique to correctly classify disaster messages, so that the classified messages can be sent to an appropriate disaster relief agency.
3. Web app development: The web app can classify and display the classification results given a input disaster message, and also display graphs of the data analysis.

In addition, this project strengthened my software skills, including the ability to create basic data pipelines and write clean, organized code.

## File Descriptions

Here's the file structure of the project:

```
| - template
| |- master.html           # main page of web app
| |- go.html               # classification result page of web app
|- run.py                  # Flask file that runs app

- data
|- disaster_categories.csv   # data to process 
|- disaster_messages.csv     # data to process
|- process_data.py
|- DisasterResponse.db     # database to save clean data to

- models
|- train_classifier.py
|- classifier.pkl          # saved model 

- README.md
```

### Run Instructions:

1. Run the following commands in the project's root directory to set up your database and model.
   - To run ETL pipeline that cleans data and stores in database `python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db`
   - To run ML pipeline that trains classifier and saves `python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl`
2. Run the following command in the app's directory to run your web app. `python run.py`
3. Go to <https://view6914b2f4-3001.udacity-student-workspaces.com/> for web application.

## Results

- With NLP techiques, machine learning pipelines, grid search for parameters optimizations, a linear model (SGD classification) was finally selected and trained. The model gives a prediction accuracy of 95%.
- The model can correctly classify the real input messages and display the classification results in the web application page as shown below.

- The graphs from the model are also displayed in the web application page. Check the screen snapshot below.
![classification](https://github.com/twang18/DSND_Projects/blob/master/2.Disaster_Response_Pipelines/classification.png)
![graphs](https://github.com/twang18/DSND_Projects/blob/master/2.Disaster_Response_Pipelines/graphs.png)

