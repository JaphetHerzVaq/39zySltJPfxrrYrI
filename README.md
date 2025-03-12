# ValueInvestor - Intelligent Stock Forecasting System

This repository contains an IPython Notebook (IPYNB) that implements an intelligent forecasting system designed to support value investing decisions in emerging markets. The project, titled **ValueInvestor**, was prepared by Japhet Hernández-Vaquero for Apziva, and is based on the specifications provided in the final project PDF.

## Project Overview

The goal of this project is to predict stock price valuations on a daily, weekly, and monthly basis using historical trading data. The system is designed to recommend **BUY**, **HOLD**, or **SELL** decisions, with an emphasis on maximizing capital returns and minimizing losses. The model does not trade on daily market volatility, but instead focuses on intrinsic value and longer-term performance. The system evaluates its effectiveness using capital return metrics and Bollinger Bands.

## Data Description

- **Input Data**: The dataset includes trading data for portfolio companies from emerging markets, with each company’s stock data provided in separate sheets. Only data from the year **2020** is used for training, and predictions are made for **2021 Q1**.
- **Key Features**: Price, Open, High, Low, Volume, and Change Percentage.
- **Preprocessing**: The notebook includes data cleaning, feature scaling, and sequence generation steps to prepare the data for model training.

## Technical Details

The notebook leverages several Python libraries, including:
- **Pandas & NumPy**: For data manipulation and numerical computations.
- **Scikit-learn**: For scaling data and evaluating model performance.
- **PyTorch**: To build and train deep learning models (LSTM networks) for time series forecasting.
- **TA and mplfinance**: For computing technical indicators and visualizing stock data.
- **Backtrader**: For backtesting trading strategies.

## How to Run

1. **Environment Setup**:  
   Install the required libraries using `pip install` (see installation commands in the notebook). Make sure you have the necessary system dependencies installed as described in the PDF.
2. **Data Import**:  
   Load the Excel file containing the stock data. The notebook reads all sheets and processes them into individual DataFrames.
3. **Preprocessing and Feature Engineering**:  
   The data is cleaned, scaled, and transformed into sequences appropriate for time series forecasting.
4. **Model Training and Prediction**:  
   An LSTM-based model is defined and trained on the 2020 data. The trained model is then used to forecast stock prices for 2021 Q1.
5. **Evaluation**:  
   The notebook visualizes the forecast versus actual stock prices and calculates residuals to evaluate model performance.

## Future Work

Future enhancements include integrating additional technical indicators, such as MACD, to improve the trading signal generation, as well as exploring alternative deep learning architectures to further enhance prediction accuracy.

## License

This project is open-source and available under the MIT License.

---

This repository serves as a comprehensive resource for anyone interested in applying deep learning techniques to financial time series analysis and value investing. Enjoy exploring the notebook and feel free to contribute with improvements and new ideas!
