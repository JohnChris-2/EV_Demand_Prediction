# EV Demand Prediction 🛠️

A predictive model project designed to forecast Electric Vehicle (EV) demand using historical data by county.

---

## 🚀 Project Overview

This repository contains code and data for predicting EV adoption trends across U.S. counties. We preprocess datasets, build and evaluate machine learning models, and save the final model for future usage or deployment.

---

## 📁 Repository Structure
EV_Demand_Prediction/

├── EV_Adoption_Forecasting.ipynb # Week 1-2 Jupyter notebook (exploration, model training, prediction, model saving)

├── forecasting_ev_model.pkl # Trained Random Forest regression model serialized via joblib

├── preprocessed_ev_data.csv # Cleaned and preprocessed dataset

├── README.md # Project description and instructions


---

## 🧠 Week 1 Progress (in Notebook)

1. **Data Loading & Exploration**  
   - Loaded raw dataset (`Electric_Vehicle_Population_Size_History_By_County_.csv`)  
   - Displayed dataset info, checked for nulls and outliers  
   - Processed date column and handled missing values (County, State)

2. **Outlier Handling**  
   - Calculated IQR for "Percent Electric Vehicles"  
   - Identified and capped outliers to reduce data skew  

3. **Preprocessing**  
   - Converted date column to datetime format  
   - Ensured no missing entries remained in key fields

---

## 🧪 Week 2 Progress (in Notebook)

1. **Feature Engineering**  
   - Prepared features and target variable for modeling

2. **Model Training and Selection**  
   - Used `RandomForestRegressor` for prediction  
   - Hyperparameter tuning via `RandomizedSearchCV`  
   - Evaluated the model using MAE, RMSE, and R² metrics

3. **Model Persistence**  
   - Saved the trained model using `joblib` to `forecasting_ev_model.pkl`

4. **Prediction Test**  
   - Loaded the saved model and tested it on sample data  
   - Verified output: actual vs. predicted EV counts

---

## 🛠️ How to Run

1. Clone the repository  
   ```bash
   git clone https://github.com/JohnChris-2/EV_Demand_Prediction.git

2. Open the notebook or create an environment with Python ≥ 3.x and install dependencies:
   pandas, numpy, scikit-learn, seaborn, matplotlib, joblib

3. Launch Jupyter Notebook and open EV_Adoption_Forecasting.ipynb
4. Run all cells sequentially to reproduce data cleaning, modeling, and saving steps

📫 Contact
Project by John Chris Prabhu
📧 Email: johnchris.work@gmail.com
