# Task 3: Energy Consumption Time Series Forecasting

## Objective
Forecast household energy consumption using historical data to optimize energy management.

## Dataset
**Household Power Consumption Dataset** containing:
- Date & Time
- Global Active Power
- Other electrical measurements

## Approach
1. **Data Loading and Preprocessing**
   - Parsed Date and Time to datetime objects.
   - Converted `Global_active_power` to numeric and handled missing values.
   - Resampled data to hourly frequency.
   - Engineered time-based features like hour of day, weekday/weekend.

2. **Train-Test Split**
   - Used 80% of data for training, 20% for testing.

3. **Forecasting Models**
   - **Prophet** for additive time series forecasting.
   - (Optional: ARIMA and XGBoost for comparison).

4. **Evaluation**
   - Compared predicted vs. actual energy usage.
   - Metrics: MAE (Mean Absolute Error) and RMSE (Root Mean Squared Error).

5. **Visualization**
   - Plotted actual vs. forecasted values.
   - Visualized trend and seasonality using Prophet components.

## Tools & Libraries
- Python, pandas, numpy, matplotlib, seaborn, Prophet, scikit-learn

## Insights
- Hourly energy usage follows clear daily and weekly patterns.
- Forecasting helps in efficient energy management and planning.
- Prophet provides easy interpretation of trends and seasonality components.
