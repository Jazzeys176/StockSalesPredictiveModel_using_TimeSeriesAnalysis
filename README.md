# Time Series Sales Forecasting with SARIMA

This project demonstrates a complete workflow for forecasting daily sales of a specific store and product family using historical sales data. The model is developed using Python and applies a Seasonal ARIMA (SARIMA) approach to capture both seasonal patterns and trends.

---

## Project Objective

The primary goal of this project is to build a time series forecasting model that can:
- Predict future sales for improved inventory and demand planning.
- Evaluate the model's accuracy and reliability using standard metrics.
- Provide actionable insights for retail management.

---

## Dataset

- **Source:** The dataset contains daily sales information for multiple stores and product families.
- **Key Columns:**
  - `date`: Date of the transaction.
  - `store_nbr`: Store number.
  - `family`: Product family.
  - `sales`: Total sales for the day.

---

## Workflow

1. **Data Preparation**
   - Filtered data for a specific store and product family.
   - Aggregated sales on a daily basis.
   - Handled missing values with forward fill to ensure data continuity.

2. **Exploratory Data Analysis**
   - Visualized sales patterns over time to identify seasonality and trends.
   - Checked for stationarity using the Augmented Dickey-Fuller test.

3. **Model Selection**
   - Performed differencing to achieve stationarity.
   - Utilized ACF and PACF plots to determine SARIMA parameters.

4. **Model Training**
   - Trained a SARIMA model using the `statsmodels` library.
   - Conducted diagnostic checks to validate model assumptions.

5. **Forecasting**
   - Forecasted sales for the next 30 days.
   - Visualized actual vs. forecasted sales for better interpretation.

6. **Model Evaluation**
   - Split the data into training and testing sets.
   - Calculated performance metrics like RMSE, MAE, and MAPE to assess model accuracy.

---

## Key Metrics
- **RMSE (Root Mean Squared Error):** Measures the standard deviation of prediction errors.
- **MAE (Mean Absolute Error):** Average magnitude of prediction errors.
- **MAPE (Mean Absolute Percentage Error):** Percentage-based error metric.

---

## Visualization

- Plots for sales trends, seasonality, and residual diagnostics.
- Forecast visualization comparing actual and predicted sales.

---

## Tools and Libraries Used

- **Python**  
- **Pandas** for data manipulation.  
- **Matplotlib** and **Seaborn** for data visualization.  
- **statsmodels** for SARIMA modeling.  
- **sklearn** for evaluation metrics.  

---

