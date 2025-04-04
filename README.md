# Air Quality Prediction (US Regions)

## Project Overview
This project explores various regression approaches to predict daily **Air Quality Index (AQI)**. Using a large dataset with features like location, pollutants, population, and seasonality, we trained and evaluated three models to see which best captures AQI trends.

## Data
- Source: Kaggle Air Quality Dataset
- Main Features: Latitude/Longitude, Defining Parameter (pollutant type), Population, Density, Date, etc.
- Size: ~5.6 million rows

## Experiments & Key Results
1. **Linear Regression**
   - RMSE: 34.53
   - Provides a baseline for performance.
2. **Ridge Regression**
   - RMSE: 34.42
   - Slight improvement; regularization didn’t fully address AQI complexity.
3. **Random Forest Regression**
   - RMSE: 30.82
   - Best performer, captures nonlinear relationships and feature interactions.

## Conclusion
- **Random Forest** achieved the most accurate predictions, indicating AQI depends on complex, nonlinear factors.
- Adding features like seasonal or location-specific interactions improved performance marginally in linear models but significantly helped ensemble methods.
