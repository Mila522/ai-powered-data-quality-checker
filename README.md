
# AI-Powered Data Quality Checker

A lightweight data engineering and machine learning application
that profiles, cleans and analyses CSV datasets.

## Features

- CSV upload and data profiling
- Missing-value and duplicate detection
- Column-name standardisation
- Missing-value imputation
- Isolation Forest anomaly detection
- Interactive data visualisations
- Downloadable cleaned datasets and anomaly reports

## Technology Stack

- Python
- Pandas
- Scikit-learn
- Streamlit
- Plotly

## Machine Learning

The application trains an Isolation Forest model on numerical
features from the cleaned dataset. It identifies unusual records
for further investigation.

An anomaly is not automatically a data error. Results require
human review.

## Data Source

Palmer Penguins dataset:
https://github.com/allisonhorst/palmerpenguins

Dataset authors: Allison Horst, Alison Presmanes Hill,
and Kristen Gorman.

## Run Locally

Create and activate a virtual environment, then install:

    pip install -r requirements.txt

Start the application:

    python -m streamlit run app.py

## Project Workflow

Raw CSV -> Data Profiling -> Cleaning -> Model Training
-> Anomaly Detection -> Export

## Future Improvements

- Automated data validation rules
- Data quality scoring
- Separate training and evaluation datasets
- Model comparison and experiment tracking
- Reusable ETL pipeline modules
