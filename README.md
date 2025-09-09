💤 Sleep Time Prediction Using Machine Learning
📌 Overview

This project predicts daily sleep hours (SleepTime) based on lifestyle and health-related factors like workout time, reading habits, phone usage, caffeine intake, work hours, and relaxation time.
The goal is to analyze data, train ML models, and compare their performance to identify the most accurate predictor.

📂 Dataset

Source: sleeptime_prediction_dataset.csv

Records: 2,000

Features: 7 (6 predictors + 1 target)

Target: SleepTime (hours of daily sleep)

Data Quality:

No missing values

No duplicate records

🔍 Features in the Dataset
Feature	Description
WorkoutTime	Daily workout time (minutes)
ReadingTime	Daily reading time (minutes)
PhoneTime	Time spent on phone (minutes)
WorkHours	Working hours per day
CaffeineIntake	Daily caffeine consumption (units)
RelaxationTime	Relaxation or leisure time (minutes)
SleepTime	Target variable (hours of sleep)
⚙️ Workflow

Data Loading & Cleaning

Imported dataset, checked duplicates, and validated data integrity.

Feature Engineering

Selected numeric features; scaled data using MinMaxScaler.

Model Training

Applied multiple regression models:

Linear Regression

SVR (Support Vector Regression)

Decision Tree Regressor

KNN Regressor

Evaluation Metrics

MAE, RMSE, R² Score used for comparison.

📊 Key Insights

Positive Influences: More workout and relaxation time lead to better sleep.

Negative Influences: High caffeine intake, long work hours, and high screen time reduce sleep.

Model Performance: Decision Tree and KNN achieved better R² scores, capturing complex patterns.

🚀 Future Improvements

Hyperparameter tuning for SVR, Decision Tree, and KNN.

Integration of biometric data for better accuracy.

Deployment as a web or mobile app for real-time predictions.

🛠️ Tech Stack

Language: Python

Libraries: pandas, numpy, sklearn, matplotlib, seaborn

Tools: Jupyter Notebook

▶️ How to Run
# Clone the repository
git clone https://github.com/yourusername/sleep-time-prediction.git

# Navigate to the folder
cd sleep-time-prediction

# Install required libraries
pip install -r requirements.txt

# Run Jupyter Notebook
jupyter notebook
