-> FUTURE_ML_01 — Sales & Demand Forecasting 
Future Interns | Machine Learning Track | Task 1

-> Objective
Build a machine learning model to forecast future store sales using historical business data, including external factors, with business-ready visualizations and actionable insights.

-> Repository Structure
FUTURE_ML_01/
├── FUTURE_ML_01_Store_Sales_Forecasting.ipynb   # Main notebook
├── eda_dashboard.png                             # EDA visualizations
├── correlation_heatmap.png                       # Feature correlations
├── model_comparison.png                          # Model performance charts
├── feature_importance.png                        # Feature importance
├── sales_forecast.png                             # Actual vs Predicted
├── future_forecast.png                            # Next 6 months forecast
└── README.md                                     # This file

-> Tools and Technology Used
| Tool                 | Purpose                 |
| -------------------- | ----------------------- |
| Python 3.x           | Core language           |
| Pandas & NumPy       | Data manipulation       |
| Matplotlib & Seaborn | Visualization           |
| Scikit-learn         | Machine learning models |
| Jupyter Notebook     | Development environment |

->  Dataset
Store Sales - https://www.kaggle.com/competitions/store-sales-time-series-forecasting

Files:
.train.csv → Main sales data
.stores.csv → Store metadata
.oil.csv → Oil prices
.holidays_events.csv → Holidays/events

Key Features:
.date, store_nbr, family
.sales (target)
.onpromotion
.External factors: oil price, holidays, store info

-> Workflow
Load Data → Clean → Feature Engineering → EDA → Model Training → Evaluation → Forecast → Insights

-> Step-by-Step Guide
🔹Data Cleaning
.Handle missing values (oil prices, promotions)
.Remove duplicates
.Ensure correct datetime format

🔹Feature Engineering
.Extract: Year, Month, Day, DayOfWeek
.Create: Lag features (lag_1, lag_7), Rolling averages, Weekend indicator
.Merge: Store metadata, Oil prices, Holidays

🔹EDA (Exploratory Data Analysis)
.Sales trends over time
.Top stores & product families
.Seasonality patterns
.Impact of promotions & holidays

🔹Model Training
.Linear Regression
.Random Forest
.Gradient Boosting

🔹Evaluation Metrics
.MAE, RMSE, R² Score, MAPE

🔹Forecasting
.Actual vs Predicted comparison
.Future 6-month sales forecast

🔹Business Insights
.Sales trends & seasonality
.Top-performing stores & products
.Promotion effectiveness
.Future demand insights

-> Models Used & Metrics

| Model             | MAE | RMSE | R² |
| ----------------- | --- | ---- | -- |
| Linear Regression | —   | —    | —  |
| Random Forest     | —   | —    | —  |
| Gradient Boosting | —   | —    | —  |
Exact values depend on your dataset run. Best model is automatically selected in the notebook.

-> Business Insights Generated
📈 Overall sales trend (growth/decline)
🏪 Top-performing stores
🛍️ High-demand product families
🎯 Promotion impact on sales
🛢️ External factor impact (oil price, holidays)
🔮 6-month future sales forecast

->How to Run
# 1. Clone the repo
git clone https://github.com/YOUR_USERNAME/FUTURE_ML_01

# 2. Install dependencies
pip install numpy pandas matplotlib seaborn scikit-learn jupyter

# 3. Launch notebook
jupyter notebook FUTURE_ML_01_Store_Sales_Forecasting.ipynb

# 4. Download dataset from Kaggle
# Place all CSV files (train, stores, oil, holidays) in the same folder

->License
This project was completed as part of the Future Interns ML Internship Program.

Made by Jeevitha | Future Interns Machine Learning Track














