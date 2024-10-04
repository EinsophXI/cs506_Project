# **Predicting Air Quality Using Weather and Traffic Data**

## **Project Overview**
This project aims to predict the Air Quality Index (AQI) of a city using real-time and historical weather conditions (e.g., temperature, humidity, wind speed) and traffic patterns (e.g., congestion, traffic flow). By leveraging machine learning models, the project provides predictions that could inform residents, urban planners, and policy makers.

---

## **Goals**
- **Goal**: Predict AQI based on weather and traffic conditions.
- **Key Features**:
  - Collect AQI, weather, and traffic data from public APIs.
  - Develop regression and time series models to forecast AQI.
  - Visualize relationships between air quality, weather, and traffic.
  - Provide reproducible results and visualizations in an interactive format.

---

## **Data Collection**
Data sources:
- **Air Quality Data**: Scraped from [OpenAQ API](https://openaq.org/).
- **Weather Data**: Gathered from [OpenWeatherMap API](https://openweathermap.org/).
- **Traffic Data**: Scraped from [Here Maps](https://developer.here.com/) or Google Maps API.

---

## **Data Processing**
1. **Cleaning**:
   - Handle missing AQI readings with time-series interpolation.
   - Standardize weather and traffic metrics for model input.
2. **Feature Engineering**:
   - Time-based features (hour, day, etc.).
   - Interaction terms between traffic congestion and weather.
   - Lagged AQI values for time series forecasting.

---

## **Modeling**
- **Machine Learning Models**:
  - Random Forest, XGBoost, and other regression models.
- **Time Series Models**:
  - LSTM and ARIMA for time-series forecasting.
- **Model Evaluation**:
  - Metrics: Mean Squared Error (MSE), R-squared.

---

## **Data Visualization**
- **Time Series Trends**: Visualize AQI trends over time.
- **Correlation Heatmap**: Show relationships between AQI, weather, and traffic.
- **Geospatial Map**: Display real-time AQI levels across the city with overlays for weather and traffic.
- **Interactive Plots**: Built using libraries like Plotly for exploration.

---

## **Test Plan**
- **Training and Testing Split**:
  - Train on data from April to September, test on October data.
- **Cross-Validation**:
  - Use k-fold cross-validation to evaluate the generalization of the models.
- **Model Performance**:
  - Track performance using MSE and R-squared on the test set.

---
