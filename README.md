# Disaster Response Pipeline Project

#Installation
Python 3.x, the following packages need to be installed for nltk:

* punkt
* wordnet
* Pipeline
* PorterStemmer
* stopwords

# Project_Motivation:
Project is a Udacity Data Scientist Nanodegree program under the data engineering, natural language processing, and machine learning skills to analyze message data that people sent during disasters to build a model for an API that classifies disaster messages. This messages could potentially be sent to appropriate disaster.

# File_Descriptions:

1.app:-
run.py: Flask file the web application.
templates contains html file for the web apps.

2.Data:-
disaster_categories.csv: dataset including all the categories.
disaster_messages.csv: dataset including all the messages.
ETL_Pipeline_Preparation.ipynb: Jupyter Notebook containing ETL pipeline scripts to read, clean, and save data into DB.
process_data.py: ETL pipeline scripts to read, clean, and save data into a DB.

3.models:-
ML_Pipeline_Preparation.ipynb: Jupyter Notebook, tokenize messages from clean data and create new columns through feature engineering. The data with new features are trained with a ML pipeline and pickled.
train_classifier.py: Script to tokenize messages from clean data and create new columns through feature engineering. The data with new features are trained with a ML pipeline and pickled

4.images:-
page 1,2,3,4,5.jpeg: screenshot of the web page 
page 6.jpeg: screenshots of the plots

# Results:
1.In ETL pipleline was built to read data from two csv files, clean data, and save data into a SQLite database.
2.Flask app was classify the message that user enters on the web page.
3.machine learning pipepline was developed to train a classifier to performs multi-output classification on the 36 categories in the Dataset.

# Instructions:
1. Run the following commands in the project's root directory to set up your database and model.

    - To run ETL pipeline that cleans data and stores in database
        `python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db`
    - To run ML pipeline that trains classifier and saves
        `python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl`

2. Run the following command in the app's directory to run your web app.
    `python run.py`

3. Go to http://0.0.0.0:3001/

# Licensing, Author, Acknowledgements

Credits must be given to Udacity for the starter codes and FigureEight for provding the data used by this project.
