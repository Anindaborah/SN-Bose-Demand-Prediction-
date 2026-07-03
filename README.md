# North-Eastern Region Electricity Demand Forecasting

This project focuses on forecasting hourly electricity demand for India's North-Eastern Region using a LightGBM regression model. The model is trained on historical demand data along with engineered time-series features to accurately predict future electricity demand.

To improve prediction performance, extensive feature engineering was performed by creating lag features and rolling statistical features. The model was further optimized using Optuna-based hyperparameter tuning with TimeSeriesSplit cross-validation, ensuring robust performance on sequential time-series data.

The final model is evaluated using standard regression metrics including MAE, RMSE, MAPE, and R², and the predictions are visualized by comparing the actual and predicted demand over the entire test period as well as the first seven days.

Features
Hourly electricity demand forecasting
Time-series feature engineering
Lag features (1h, 24h, 48h, 168h, 336h)
Rolling mean, standard deviation, maximum, and minimum features
LightGBM regression model
Hyperparameter optimization using Optuna
TimeSeriesSplit cross-validation
Model evaluation using MAE, RMSE, MAPE, and R²
Visualization of actual vs. predicted electricity demand
Tech Stack
Python
Pandas
NumPy
LightGBM
Optuna
Scikit-learn
Matplotlib
Results

The tuned LightGBM model provides accurate hourly demand forecasts by leveraging historical demand patterns and optimized model parameters. Hyperparameter optimization significantly improved the model's predictive performance compared to the baseline model.
