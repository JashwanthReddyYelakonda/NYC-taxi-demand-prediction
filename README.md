# NYC Taxi Demand Prediction with Machine Learning

This project focuses on predicting hourly taxi demand across New York City by using historical Yellow Taxi trip data and hourly weather data from January to March 2023. By combining ride records with weather features, machine learning models are trained to uncover demand patterns. The objective is to improve fleet efficiency, reduce passenger wait times, and support data-driven decisions for urban transportation planning.

---

## Project Features

### Objective  
Develop a machine learning-based forecasting system to predict taxi demand for the next hour in different boroughs of New York City, incorporating both historical ride and weather data.

---

## Dataset

- **Taxi Data**: Trip records from the NYC Taxi & Limousine Commission (TLC)  
- **Weather Data**: Hourly weather conditions (temperature, wind, precipitation, visibility) from Visual Crossing

---

## Data Preprocessing

- Removal of invalid records (e.g., trips with duration over 12 hours or speeds over 60 mph)  
- Cleaning and merging weather data with trip data by hour  
- Feature engineering including:
  - Trip metrics: duration, average speed  
  - Time breakdown: hour, weekday, month  
  - Weather summaries: temperature, wind, precipitation

---

## Model Architectures

- LightGBM  
- CatBoost  
- XGBoost  
- AdaBoost  

All models are trained to forecast the number of rides in the next hour (`rides_next_hour`) and are evaluated using regression metrics.

---

## Evaluation Metrics

- **MAE**: Mean Absolute Error  
- **MSE**: Mean Squared Error  
- **RMSE**: Root Mean Squared Error

---

## Project Structure

NYC-taxi-demand-prediction/
├── data/ # Contains weather CSV files
├── notebooks/ # Jupyter notebooks for analysis and modeling
├── README.md # Project documentation
└── .gitignore

---

## Project Impact

- Improved fleet allocation efficiency  
- Shorter passenger wait times  
- Better use of weather and time-based demand patterns  
- Foundation for future real-time forecasting

---

## Author

**Jashwanth Reddy Yelakonda**  
MS in Information Systems, Murray State University  
Graduate Assistant, SDS Center

---

## References

- [NYC TLC Trip Data](https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page)  
- [Visual Crossing Weather](https://www.visualcrossing.com/)  
- Viswanath, D. (2022). *NYC Taxi Demand Prediction Using Machine Learning*. [Medium Article](https://medium.com/analytics-vidhya/new-york-yellow-taxi-demand-prediction-using-machine-learning-fc697d20ff86)  
- Chou, K. S., et al. (2023). *Taxi Demand and Fare Prediction with Hybrid Models*. Applied Sciences, 13(18), 10192.
