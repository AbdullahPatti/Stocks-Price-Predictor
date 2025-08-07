Stock Price Predictor
Overview
The Stock Price Predictor is a Python-based machine learning project that forecasts stock prices for major companies using historical data. This project uses a Linear Regression model to predict future closing prices based on 60-day sequences of historical stock prices. It leverages the yfinance library to fetch real-time stock data and includes data preprocessing, model training, evaluation, and prediction visualization. The project is implemented in a Jupyter Notebook, making it easy to follow and extend.
Features

User Input: Select from a list of 10 popular companies (e.g., Apple, Microsoft, NVIDIA) via a simple numbered menu.
Data Retrieval: Downloads historical stock data from Yahoo Finance using yfinance from January 1, 2020, to the current date.
Data Preprocessing: Normalizes stock prices and creates 60-day sequences for time-series prediction.
Model: Uses a Linear Regression model from scikit-learn for simplicity and interpretability.
Evaluation: Computes Mean Squared Error (MSE), Mean Absolute Error (MAE), and R² Score to assess model performance.
Predictions: Forecasts stock prices for the next 30 days, displayed in a user-friendly format.

Requirements
To run this project, you need the following Python libraries:

pandas
numpy
matplotlib
seaborn
yfinance
scikit-learn

You can install them using pip:
pip install pandas numpy matplotlib seaborn yfinance scikit-learn

Installation

Clone this repository to your local machine:git clone https://github.com/your-username/stock-price-predictor.git


Navigate to the project directory:cd stock-price-predictor


Install the required dependencies:pip install -r requirements.txt


Ensure you have Jupyter Notebook installed:pip install jupyter



Usage

Open the Jupyter Notebook:jupyter notebook Stock_Predictor.ipynb


Run the cells in sequence:
The first cell imports necessary libraries.
The second cell prompts you to select a stock by entering a number (1-10).
Subsequent cells fetch data, preprocess it, train the model, evaluate performance, and display predictions.


When prompted, enter a number corresponding to a company (e.g., 7 for NVIDIA).
The notebook will output:
The selected ticker symbol.
Model performance metrics (MSE, MAE, R² Score).
Predicted stock prices for the next 30 days.



Note: The notebook assumes an active internet connection to fetch data via yfinance.
Project Structure

Stock_Predictor.ipynb: The main Jupyter Notebook containing the code.
README.md: This file, providing project documentation.
(Optional) requirements.txt: Lists dependencies for easy installation.

Example Output
For NVIDIA (NVDA), the model might produce:
Mean Squared Error (MSE): 0.0009
Mean Absolute Error (MAE): 0.0222
R² Score: 0.9219

Sample predictions:
2025-08-07: $183.09
2025-08-08: $182.74
...
2025-09-05: $210.82
This project is licensed under the MIT License. See the LICENSE file for details.
Contact
Feel free to reach out with questions or suggestions! Connect with me on LinkedIn or open an issue on this repository.
