📊 FMCG Sales Forecasting and Profitability Analysis using ML, DL, and Time Series Modeling
👨‍💻 Project Objective
The goal of this project is to build an end-to-end data science solution for forecasting FMCG sales for the next 2 months and analyzing profitability patterns across different regions and products. This includes:

Preprocessing and EDA

Machine Learning & Deep Learning models

Time Series forecasting using STL and SARIMA

Visualizations for strategic decision-making

Hyperparameter tuning and model evaluation (overfitting/underfitting)

Business insights and competitive strategy suggestions

📂 Step 1: Data Preprocessing
Dataset: FMCG sales data containing features like Date, Product, Region, Sales_Channel, Sales_Units, Profit_Percent, Discount_Percent, and Stock_Available.

Steps performed:

Handled datetime parsing and sorting

Label encoded categorical variables

Scaled numerical features using MinMaxScaler

Created scaled_sales for DL models

📈 Step 2: Exploratory Data Analysis (EDA)
Sales Trend Over Time: Visualized using line plots to observe overall movement.

Product-Wise Sales: Visualized using pie charts showing the contribution of each product.

Region-Wise Stock Availability: Donut chart revealed regions with high inventory.

Profitability vs Region Analysis: Planned to identify high-profit zones and compare them with competitors.

🧠 Step 3: Machine Learning Models
Models used:

Random Forest

Ridge Regression

Support Vector Regressor (SVR)

Cross-validation: TimeSeriesSplit was used to maintain temporal integrity.

Evaluation Metrics: R² Score, MSE

Insights:

Random Forest generally performed well on the sales prediction task.

Hyperparameter tuning can be added using GridSearchCV or Optuna.

⚙️ Step 4: Hyperparameter Tuning
Planned to implement:

GridSearchCV / RandomizedSearchCV for ML models

Epoch and learning rate tuning for DL models

🧠 Step 5: Deep Learning Models
Used LSTM, GRU, and Dense (fully connected) models on time series windows:

Window size: 30 days

Evaluation: Compared with actual test data using R² scores

Overfitting vs Underfitting:

Loss vs Val Loss plots to detect overfitting

Apply regularization/dropout to mitigate

⏳ Step 6: Time Series Forecasting
STL Decomposition:

Broke sales into trend, seasonality, and residuals

Helps in detecting seasonal demand patterns

SARIMA Model:

Forecasted next 60 days (2 months)

Captured both trend and seasonality

📌 Step 7: Advanced Forecasting Ideas
You may further improve this section using:

ARIMA, SARIMA+Exog for external features like promotions

Facebook Prophet

XGBoost / LGBM with lag features

📊 Step 8: Model Performance Comparison
A bar chart compared R² scores across all models (ML and DL), providing a quick visual insight into:

Which model performs best

Trade-offs between complexity and performance

🏙️ Step 9: Business Insights and Strategy
➤ District-Level Profitability Analysis
Analyze regions with high profit percent and high sales units

Visualize via heatmaps or grouped bar plots

Identify underperforming regions where competitor products are dominating

➤ Strategic Suggestions:
Invest in promotions/discounts in low-profit regions

Increase stock availability in high-performing regions

Launch region-specific products or bundles

Use A/B testing for campaigns in target zones

📉 Step 10: Overfitting & Underfitting Analysis
Plotted training vs validation loss to detect model behavior

Used dropout in DL models to reduce overfitting

Planned to add early stopping & regularization

🔍 Step 11: Future Work
Add LightGBM and XGBoost models

Integrate external datasets like holidays, promotions

Build a dashboard using Streamlit or Power BI

Deploy using Flask/Streamlit with a predictive service

✅ Conclusion
This project not only built robust forecasting models but also translated the insights into actionable business strategies. By using time series, machine learning, and deep learning together, we achieved a well-rounded understanding of both the "what" and the "why" behind sales trends, positioning this solution as a decision-making tool for FMCG businesses.
