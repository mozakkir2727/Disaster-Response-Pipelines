# Disaster Response Pipeline Project

# Instructions:

1. Run the following commands in the project's root directory to set up your database and model.

    * To run ETL pipeline that cleans data and stores in database:-
        "python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db"

    * To run ML pipeline that trains classifier and saves:-
        "python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl"

2. Run the command inside the app's directory to run your web app.
    "python run.py"

3. Go to https://view6914b2f4-3001.udacity-student-workspaces.com
