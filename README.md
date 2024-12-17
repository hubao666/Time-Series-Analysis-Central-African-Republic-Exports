# Time-Series-Analysis-Central-African-Republic-Exports
## Topic
The study analyzes the Central African Republic's export data (1960–2017) using time series analysis to identify trends and forecast future values, supporting economic planning.

## Methodology
- Data Preprocessing: Cleaned data and confirmed no missing values.
- Stationarity: ADF tests showed the data was non-stationary. First-order differencing achieved stationarity.
- Model Selection:
  - ACF/PACF plots suggested MA(1) and AR(2) on differenced data.
  - Diagnostics (AIC, BIC, and Ljung-Box test) favored AR(2).
  - Machine Learning Method: Split data into training/testing sets; ARMA(1,2) was chosen based on the lowest MSE.
## Tools
- Python for analysis and visualization.
- Models: AR(2), MA(1), ARMA(1,2).
- Metrics: AIC, BIC, MSE.
## Results
- AR(2) and ARMA(1,2) were selected as the best models.
$$
y_t = -0.505033 y_{t-1} -0.289666 y_{t-2}+ w_t
$$

$$
y_t = 0.337728 y_{t-1} -0.883232 w_{t-1}+ 0.441870w_{t-2} + w_t
$$
- Forecasts for 2018–2021 show export values stabilizing around 12.6 million USD.
