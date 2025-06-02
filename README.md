NYC Taxi Demand Prediction with Machine Learning
This project focuses on predicting hourly taxi demand across New York City by using historical Yellow Taxi trip data and hourly weather data from January to March 2023. By combining ride records with weather features, machine learning models are trained to uncover demand patterns. The objective is to improve fleet efficiency, reduce passenger wait times, and support data-driven decisions for urban transportation planning.

Project Features
Objective
Develop a machine learning-based forecasting system to predict taxi demand for the next hour in different boroughs of New York City, incorporating both historical ride and weather data.

Dataset
Taxi Data: Trip records from the NYC Taxi & Limousine Commission (TLC)

Weather Data: Hourly weather conditions (temperature, wind, precipitation, visibility) from Visual Crossing

Data Preprocessing
Removal of invalid records (e.g., trips with duration over 12 hours or speeds over 60 mph)

Cleaning and merging weather data with trip data by hour

Feature engineering including:

Trip metrics: duration, average speed

Time features: hour, weekday, month

Weather summaries for each pickup hour

Model Architectures
LightGBM

CatBoost

XGBoost

AdaBoost

All models are trained to forecast rides_next_hour, and their predictions are compared using standard evaluation metrics.

Evaluation Metrics
MAE: Mean Absolute Error

MSE: Mean Squared Error

RMSE: Root Mean Squared Error

Each model’s performance is compared based on these regression metrics to select the best-performing approach.

Project Directory Structure
graphql
Copy
Edit
NYC-taxi-demand-prediction/
├── data/             # Contains raw CSV files (weather data)
├── notebooks/        # Jupyter notebook(s) for data analysis and model training
├── presentation/     # Final PowerPoint presentation for the project
├── README.md         # Project overview and documentation
└── .gitignore
Project Impact and Insights
More efficient taxi allocation by identifying peak demand areas and times

Reduced waiting times for passengers

Improved operational planning for fleet managers

Insights into the influence of weather and temporal variables on taxi demand

Foundation for future integration of real-time traffic and weather APIs

Author
Jashwanth Reddy Yelakonda
Master of Science in Information Systems
Murray State University
Graduate Assistant, SDS Center

References
NYC TLC Trip Data: https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page

Visual Crossing Weather: https://www.visualcrossing.com/

Viswanath, D. (2022). New York Yellow Taxi Demand Prediction Using Machine Learning. https://medium.com/analytics-vidhya/new-york-yellow-taxi-demand-prediction-using-machine-learning-fc697d20ff86

Chou, K. S., et al. (2023). Taxi Demand and Fare Prediction with Hybrid Models. Applied Sciences, 13(18), 10192.