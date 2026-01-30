### Bakery Demand Forecasting System

A scalable time-series forecasting system designed for a large retail bakery managing 1,200+ products across multiple branches. The system captures heterogeneous demand patterns, temporal trends, and special-day seasonality to generate accurate, branch-specific forecasts for inventory planning and promotions.

##Features

- **Temporal & Calendar Features**: Month, day, weekday, weekends, month start/end flags.

- **Domain-Specific Seasonality**: Captures demand spikes for Ramadan, Eid, Valentine’s Day, Independence Day, and other cultural events.

- **Lagged & Rolling Features**: Incorporates past sales and moving averages to capture trends.

- **Transformations**: Log transforms applied to stabilize variance.

- **Hyperparameter-Tuned Models**: Separate Random Forest models per product–branch, optimized via grid search.

- **Custom Evaluation**: Hybrid Weighted Mean Directional Accuracy (WMDA) + RMSE metric (α=0.9, β=0.1) for model selection.

- **Rolling Window Validation & Calibration**: Ensures robust performance and avoids overfitting.

- **Forecast Uncertainty**: Supports calibrated confidence intervals for better inventory risk management.
