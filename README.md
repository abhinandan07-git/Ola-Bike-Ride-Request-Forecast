
#  🚲 Ola Bike Ride Request Forecast

## 📌 Overview

This project focuses on predicting bike ride request demand using historical data from Ola. The goal is to build a machine learning model that can accurately forecast ride demand based on temporal, weather, and contextual features.

Such predictions can help in:

* Efficient fleet management
* Reducing rider wait times
* Improving resource allocation
## 📂 Project Structure

```
├── data/
│   └── ola.csv
├── notebook/
│   └── Ola_Bike_Ride_Request_Forecast.ipynb
├── images/
│   └── (EDA plots)
├── README.md                      
```

## 📂 Dataset

The dataset contains ride request information along with features such as:

* Datetime
* Season
* Weather conditions
* Temperature
* Humidity
* Windspeed
* User type (casual/registered)
* Ride count (target variable)



## 🚀 Installation

### 1️⃣ Clone the repository:

```bash
https://github.com/abhinandan07-git/Ola-Bike-Ride-Request-Forecast.git

```

### 2️⃣ Install dependencies:

Ensure you have the following Python packages installed:

- `RandomForest`
- `LinearRegression`
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `xgboost`
- `SVM` 

Install them with:

```bash
pip install 
```

## 🔍 ⚙️ Project Workflow

1. Data Preprocessing

* Loaded dataset using pandas
* Checked shape, data types, and summary statistics
* Handled missing values using mean imputation

2. Feature Engineering

* Extracted:
    * Year, month, day from datetime
    * Hour from time
* Created new features:
    * Weekday/weekend indicator
    * AM/PM classification
    * Holiday indicator using holidays library
* Dropped unnecessary columns:
    * datetime, date

⸻

3. Exploratory Data Analysis (EDA)

* Distribution plots for numerical features
* Boxplots to detect outliers
* Correlation heatmap to identify relationships
* Analysis of ride demand across:
    * Time
    * Month
    * Weather conditions

⸻

4. Data Cleaning

* Handled outliers in:
    * Windspeed
    * Humidity
* Removed highly correlated or redundant features

⸻

5. Model Building

Split dataset into training and validation sets.

Applied feature scaling using:

* StandardScaler

Trained multiple models:

* Linear Regression
* Lasso Regression
* Ridge Regression
* Random Forest Regressor
* XGBoost Regressor

⸻

6. Model Evaluation

Models were evaluated using:

* Mean Absolute Error (MAE)

Comparison of multiple models helped identify the best-performing approach.

⸻

🧠 Key Insights

* Ride demand is strongly influenced by:
    * Time of day
    * Weather conditions
    * Seasonal patterns
* Feature engineering significantly improved model performance
* Ensemble models like Random Forest and XGBoost performed better than linear models

⸻

🛠️ Tech Stack

* Programming Language: Python
* Libraries:
    * pandas, numpy
    * matplotlib, seaborn
    * scikit-learn
    * xgboost
    * holidays

## 📊 Visualizations

Some visualizations generated during the analysis include

<img width="1229" height="992" alt="image" src="https://github.com/user-attachments/assets/7f60716c-efac-40c7-9d00-885afb375643" />
     check for any relation between the ride request count with respect to the day, time, or month
<img width="1617" height="860" alt="image" src="https://github.com/user-attachments/assets/4125ae2e-528d-4d80-90c7-3fe07fc01f44" />
      visualising  , season , weather , holidays,
            am_or_pm, year, weekday
<img width="1253" height="453" alt="image" src="https://github.com/user-attachments/assets/05b9e27d-95ea-4ecc-9a8d-04a38473b3a4" />
     visualising temp. and windspeed
<img width="1249" height="434" alt="image" src="https://github.com/user-attachments/assets/3545d440-9b86-4d65-b891-3062cc5e826b" />
     irregularities in  the data distribution
<img width="1249" height="819" alt="image" src="https://github.com/user-attachments/assets/8dc677f1-833c-455c-945b-ec1dce3e46e1" />

<img width="600" height="474" alt="image" src="https://github.com/user-attachments/assets/ac531deb-9e59-4117-bbdd-7115e1b98ee3" />                                                              correlated features in our dataset 



## 🛠️ Tech Stack

* Programming Language: Python
* Libraries:
    * pandas, numpy
    * matplotlib, seaborn
    * scikit-learn
    * xgboost
    * holidays

## 📈 Future Improvements

* Hyperparameter tuning for better accuracy
* Time-series specific models (ARIMA, LSTM)
* Deployment as a web app (Flask/Streamlit)
* Real-time demand prediction.
