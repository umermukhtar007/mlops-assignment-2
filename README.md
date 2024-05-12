# Airflow Data Extraction Pipeline
This project automates a data extraction lifecycle from extracting data, transforming it, saving it while versioning the data with dvc and code with git.

## How To Run?
- Install the necessary libraries from `requirements.txt` file
- Run followiung to install airflow in python virtual environment
```
pip install apache-airflow
```

- Run following to set airflow environment variable
```
export AIRFLOW_HOME="root of this cloned repo"
```

- Run following to initialize airflow database
```
airflow db init
```

- Run following in a seperate console which tracks changes in dags
```
airflow scheduler
```

- Run follwing in a seperate console and open airflow user interface at `http://localhost:8080`
```
airflow webserver -p 8080
```

- Find the dag with the name specified in the code and toggle the pause button to activate the dag
- Click play button on top right to manually trigger the dag run.
