# ARIMAX Solar Power Generation Forecasting

This is a Python-based ARIMAX (AutoRegressive Integrated Moving Average with Exogenous Variables) model for forecasting the intensity of sunlight radiation using sensor data from the dataset available at https://www.kaggle.com/datasets/anikannal/solar-power-generation-data. The primary libraries utilized in this project are sklearn, statsmodels, numpy, pandas, matplotlib, and pmdarima.

## Dataset

The dataset used for this project contains solar power generation data, including sensor readings, such as ambient temperature, module temperature, and irradiation levels. The data is collected from two solar power plants located in different regions of India. The dataset is available in CSV format and is loaded into a pandas DataFrame for further processing.

## Objective

The objective of this project is to develop a forecast model that can predict the intensity of sunlight radiation using the available sensor data. The ARIMAX model is employed to account for the potential impact of exogenous variables, such as temperature and irradiation levels, on the sunlight radiation intensity.

## Dependencies

The following Python libraries are used in this project:

1. `sklearn`: Provides machine learning functionalities, such as data preprocessing, model training, and model evaluation.
2. `statsmodels`: Offers advanced statistical modeling capabilities, including time series analysis and forecasting.
3. `numpy`: Provides support for numerical computations, such as array manipulation and mathematical operations.
4. `pandas`: Offers data manipulation and analysis tools, including data cleaning, transformation, and aggregation.
5. `matplotlib`: Provides visualization capabilities for creating plots and charts to visualize data and model results.
6. `pmdarima`: Offers an implementation of the AutoRegressive Integrated Moving Average (ARIMA) model with automatic selection of model hyperparameters.

## Model Building

The ARIMAX model is implemented using the following steps:

1. Data Preparation: The dataset is loaded into a pandas DataFrame and preprocessed to handle any missing values or outliers. The relevant columns for the ARIMAX model, such as sunlight radiation intensity, ambient temperature, module temperature, and irradiation levels, are extracted and stored in separate arrays.
2. Feature Engineering: The exogenous variables, such as ambient temperature, module temperature, and irradiation levels, are used as additional features in the ARIMAX model.
3. Model Training: The ARIMAX model is trained using the preprocessed data. The appropriate hyperparameters for the ARIMA model, such as the order of differencing (d), the order of autoregression (p), and the order of moving average (q), are automatically selected using the `pmdarima` library. The exogenous variables are also provided as input to the ARIMAX model during the training process.
4. Model Prediction: Once the ARIMAX model is trained and evaluated, it can be used for making future predictions of the sunlight radiation intensity based on the exogenous variables. The model can be used to forecast the intensity of sunlight radiation at various time horizons, depending on the requirement.

## Results

The ARIMAX model developed in this project provides accurate predictions of the intensity of sunlight radiation based on the available sensor data. The model takes into account the potential impact of exogenous variables, such as ambient temperature, module temperature