# Stock_price_Prediction

## Stock Price Prediction using Linear Regression

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-1.2.2-orange)
![License](https://img.shields.io/badge/License-MIT-green)

A machine learning project that predicts stock closing prices using historical market data and Linear Regression.


## Dataset
- Source: <Add data source (e.g., Yahoo Finance, Kaggle)>
- Contains:
  - Open price
  - High price
  - Low price
  - Volume
  - Close price (target variable)
  
Example data structure:


## **Import Libraries:**
The project uses several Python libraries, including:
  * `pandas`: for data manipulation and analysis.
  * `yfinance`: for downloading financial data.
  * `datetime`: for handling dates and times.
  * `matplotlib` and `seaborn`: for data visualization.
  * `scikit-learn`: for machine learning algorithms.


## Data Acquisition and Preprocessing
- The code downloads historical stock data for Google (GOOG) from Yahoo Finance for the past 100 months.
- It handles missing values using forward and backward fill, and removes any remaining null values.
- Data normalization/scaling is done using `MinMaxScaler`.

## Exploratory Data Analysis (EDA)

- Visualizes stock prices over time.
- Calculates and visualizes daily returns.
- Displays a histogram of daily returns to observe the distribution.

## Model Training and Evaluation

Several regression models are trained and evaluated using R-squared as the primary metric:

* Linear Regression
* Ridge Regression
* Lasso Regression
* Random Forest Regressor
* Support Vector Regression

The model with the highest R-squared score is selected as the best model.  Other evaluation metrics include Mean Absolute Error (MAE), Mean Squared Error (MSE), and Root Mean Squared Error (RMSE).

## Prediction

The best model is used to predict the closing price of the stock for the next day. 

## Visualization

A scatter plot visualizes the relationship between actual and predicted prices for the test set.

## Usage

Run the Python script to execute the entire process.  The predicted stock price for the next day will be printed to the console.

## Future Improvements:

* **More Features:** Incorporate additional features such as moving averages, technical indicators, or economic data.
* **Hyperparameter Tuning:** Optimize model parameters for better performance.
* **Ensemble Methods:** Combine predictions from multiple models.
* **Real-time Data Integration:**  Fetch real-time data for more up-to-date predictions.
* **Different Stock Symbols**: Add more ticker symbols to test the models performance on a wider variety of stocks.



