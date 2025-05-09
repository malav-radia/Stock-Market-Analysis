
# Stock Market Price Predictor

This project is a web-based application that predicts future stock prices using a deep learning model built with Keras. It utilizes historical stock data retrieved from Yahoo Finance and provides users with visualizations and predictions to aid investment insights.

## Tech Stack

- Python  
- Streamlit – for creating the web app interface  
- Keras/TensorFlow – for building and loading the prediction model  
- yfinance – for fetching real-time historical stock data  
- Matplotlib – for plotting stock price trends and predictions  
- Scikit-learn – for data preprocessing  

## Features

- Input any valid stock ticker (e.g., `GOOG`, `AAPL`) to analyze  
- Visualize raw stock prices along with 50, 100, and 200-day moving averages  
- Predict future stock prices using a trained LSTM model  
- Compare predicted prices against the actual values using interactive charts  

## Model Details

- The LSTM model is trained on the stock's closing prices  
- Data is normalized using MinMaxScaler  
- Uses a 100-day look-back window for predictions  
- Predictions are rescaled to their original value for display  

## How to Run the App

1. Clone the repository:  
   ```bash
   git clone https://github.com/your-username/stock-market-predictor.git  
   cd stock-market-predictor  
   ```

2. Install required packages:  
   ```bash
   pip install -r requirements.txt  
   ```

3. Launch the app:  
   ```bash
   streamlit run app.py  
   ```

4. Enter a stock symbol and visualize its trends and predictions.

## Files Included

- `app.py` – Main Streamlit web app  
- `StockPrediction.ipynb` – Jupyter Notebook with model training and exploration  
- `Stock Prediction Model.keras` – Pre-trained Keras model for stock prediction  

## Notes

- Ensure an active internet connection for fetching data via yfinance  
- The app currently loads the model from a local path; modify the model path if needed when deploying  

