# disaster_response_pipeline_project
### Instructions:
1. Run the following commands in the project's root directory to set up your database and model.

    - To run ETL pipeline that cleans data and stores in database
        `python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db`
    - To run ML pipeline that trains classifier and saves
        `python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl`

2. Run the following command in the app's directory to run your web app.
    `python run.py`

3. Go to http://0.0.0.0:3001/


Here's the file structure of the project:

```
- app
| - template
| |- master.html  # main page of web app
| |- go.html  # classification result page of web app
|- run.py  # Flask file that runs app

- data
|- disaster_categories.csv  # data to process 
|- disaster_messages.csv  # data to process
|- process_data.py
|- InsertDatabaseName.db   # database to save clean data to

- models
|- train_classifier.py
|- classifier.pkl  # saved model 

- README.md
```

Due to size limitation of Github, classifier.pkl is kept in the Google Share Drive
https://drive.google.com/drive/folders/13s52ZwrHu_d90-HG33C0o2t1x3OhanLM?ogsrc=32

### Front End App
![Home Page](https://github.com/SmokeShine/disaster_response_pipeline_project/blob/master/app/FrontEnd1.png)
### Message Categorization
![Categorization](https://github.com/SmokeShine/disaster_response_pipeline_project/blob/master/app/FrontEnd2.png)