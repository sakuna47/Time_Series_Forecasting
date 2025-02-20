# # Time Series Forecasting with ARIMA and Prophet

This project demonstrates time series forecasting using ARIMA and Prophet models on the airline passengers dataset. It includes model training, evaluation, visualization, and deployment using Streamlit.

## Features
- Data loading and preprocessing
- ARIMA model implementation and evaluation
- Prophet model implementation and evaluation
- Model saving using Joblib
- Deployment with Streamlit for interactive forecasting

## Installation

Ensure you have the necessary dependencies installed. Run the following command:

```sh
pip install --upgrade pip setuptools wheel
pip install pystan==2.19.1.1
pip install prophet
pip install pandas numpy matplotlib statsmodels tensorflow scikit-learn joblib streamlit
```

## Dataset

The dataset used is the **Monthly Airline Passengers Dataset**, available from [here](https://raw.githubusercontent.com/jbrownlee/Datasets/master/airline-passengers.csv).

## Usage

### Train Models
1. Run the Python script to train ARIMA and Prophet models:
   ```sh
   python train_models.py
   ```
2. This will save the trained models in Google Drive (if running in Google Colab) or locally.

### Run Streamlit App
To launch the interactive forecasting app using Streamlit:

```sh
streamlit run app.py
```

## Project Structure
```
📂 time-series-forecasting
│── 📄 train_models.py       # Script for training ARIMA and Prophet models
│── 📄 app.py                # Streamlit app for interactive forecasting
│── 📂 models/               # Folder for storing saved models
│── 📄 README.md             # Project documentation
```

## Model Evaluation
### ARIMA Model
- Trained with order (5,1,0)
- Evaluated using Mean Squared Error (MSE) and Mean Absolute Error (MAE)

### Prophet Model
- Automatically detects seasonality and trends
- Forecasts future values with confidence intervals

## Deployment
The project includes a **Streamlit** web application that allows users to visualize historical and predicted data interactively.

## Acknowledgments
- Dataset sourced from [Jason Brownlee's repository](https://github.com/jbrownlee/Datasets)
- Prophet model by Facebook

## License
This project is licensed under the MIT License.

