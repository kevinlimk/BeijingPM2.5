# Beijing PM2.5

This study uses recorded [PM2.5 concentration data in Beijing](https://archive.ics.uci.edu/ml/datasets/PM2.5+Data+of+Five+Chinese+Cities) from 2010 to 2015 to construct a time series forecast that can predict daily PM2.5 concentration. Such a model could provide citizens a means of anticipating fluctuations in air quality in order to minimize exposure to air pollutants on days with especially high PM2.5 concentration level.

The time series forecast employs ARIMA and LSTM models.

This project is organized into 3 Jupyter Notebooks:

* [01_datawrangling.ipynb](https://github.com/kevinlimk/BeijingPM2.5/blob/master/01_datawrangling.ipynb) - Data cleaning to generate cleaned daily and hourly PM2.5 concentration data.
* [02_eda.ipynb](https://github.com/kevinlimk/BeijingPM2.5/blob/master/02_eda.ipynb) - Exploratory data analysis to examine  hourly, weekly, and monthly trends in PM2.5 concentration along with correlations to temperature, pressure, humidity, dew point, and precipitation.
* [03_featureengineering.ipynb](https://github.com/kevinlimk/BeijingPM2.5/blob/master/03_machinelearning.ipynb) - Machine learning using ARIMA and LSTM models to construct time series forecasts.
  
Installation
---

Assuming that Python 3 and Jupyter Notebook are already installed:

  * Clone the BeijingPM2.5 repo.
  * Navigate to the BeijingPM2.5 directory and run venv: `python3 -m venv env`
  * Activate the virtual environment: `source env/bin/activate`
  * Install the Python requirements: `pip install -r requirements.txt`
