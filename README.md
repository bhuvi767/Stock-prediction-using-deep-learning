# Stock Market Forecasting App

## Overview

The Stock Market Forecasting App is a web application built using Streamlit that allows users to forecast stock market prices of selected companies. The app leverages multiple forecasting models including SARIMA, Random Forest, LSTM, and Prophet to provide predictions based on historical stock data.

## Features

- Interactive user interface to select stock symbols and date ranges.
- Data visualization of historical stock prices.
- Stationarity check using the ADF test.
- Decomposition of time series data into trend, seasonality, and residuals.
- Forecasting using SARIMA, Random Forest, LSTM, and Prophet models.
- Comparison of actual vs. predicted stock prices.
Install the required packages:

bash

pip install -r requirements.txt

Run the application:

bash

    streamlit run app.py

Usage

    Open the app in your web browser. You should see the title "Stock Market Forecasting App".
    Use the sidebar to select the start and end dates for the historical data.
    Choose a company from the dropdown list to fetch its stock data.
    View the fetched data and its visualization in the main panel.
    Select the column you want to use for forecasting.
    Check the stationarity of the data and decompose it to understand its components.
    Choose a forecasting model from the sidebar.
        SARIMA: Select parameters p, d, q, and seasonal order, and set the forecast period.
        Random Forest: The model automatically splits the data and provides RMSE.
        LSTM: Set the sequence length for LSTM, train the model, and view the predictions.
        Prophet: Automatically fits the model and forecasts for a future period.
    View the forecast results and compare them with actual data.

Dependencies

    streamlit
    yfinance
    pandas
    numpy
    matplotlib
    seaborn
    plotly
    statsmodels
    fbprophet
    scikit-learn
    keras

File Structure

stock-market-forecasting-app/
├── app.py
├── requirements.txt
└── README.md

Models Used
SARIMA

    Seasonal AutoRegressive Integrated Moving Average (SARIMA) model for time series forecasting.
    User can select parameters p, d, q, and seasonal order for model tuning.

Random Forest

    Ensemble learning method for regression.
    Automatically splits data into training and testing sets.
    Provides RMSE for model evaluation.

LSTM

    Long Short-Term Memory (LSTM) neural network for sequence prediction.
    Scales data and creates sequences for training.
    User can set the sequence length for the model.

Prophet

    Facebook's Prophet model for time series forecasting.
    Handles seasonality and trends in the data.
    Automatically fits the model and provides future forecasts.


Acknowledgments

    The app uses Yahoo Finance for fetching historical stock data.
    Image from Freepik used in the app.


