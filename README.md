# Task 05 – Time-Series Forecasting with ARIMA

## Objective
Analyze daily demand, inspect trend and weekly seasonality, test stationarity, train an ARIMA model, evaluate it using RMSE and MAPE, and produce a 30-day forecast.

## Dataset
`data/daily-demand-series.csv` contains 30 daily observations with columns:
- `date`
- `demand`
- `marketing_event`
- `holiday`

## Project structure
```text
task05_time_series_forecasting/
├── data/
│   └── daily-demand-series.csv
├── notebooks/
│   └── task05_time_series_forecasting.ipynb
├── requirements.txt
└── README.md
```

## Setup
From the project root, install dependencies:
```bash
python -m pip install -r requirements.txt
```

Open the notebook:
```bash
jupyter notebook
```
Then open `notebooks/task05_time_series_forecasting.ipynb` and run all cells from top to bottom.

## Methods
1. Data inspection and cleaning
2. Exploratory data analysis
3. Additive decomposition with a 7-day period
4. Augmented Dickey-Fuller stationarity test
5. First-order differencing
6. ARIMA order selection using AIC
7. Train/test evaluation using RMSE and MAPE
8. 30-day forecast with confidence intervals

## Important limitation
The supplied dataset contains only 30 observations. Forecasts are exploratory and should not be treated as highly reliable long-term predictions. The supplied `marketing_event` and `holiday` features are inspected but are not used in the univariate ARIMA model.
