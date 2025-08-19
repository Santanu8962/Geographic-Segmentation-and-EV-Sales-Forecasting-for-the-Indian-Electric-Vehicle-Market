# Geographic-Segmentation-and-EV-Sales-Forecasting-for-the-Indian-Electric-Vehicle-Market

This project presents a data-driven analysis and forecasting framework for the Indian Electric Vehicle (EV) market using geographic segmentation and machine learning.

We use state-wise EV sales data (2014–2024) to identify adoption patterns and predict short-term EV demand.

🔹 Objectives

Perform geographic segmentation of EV adoption across Indian states.

Identify high-potential regions and vehicle categories (2W, 3W, 4W, Bus, Others).

Build a forecasting model for short-term EV sales using XGBoost with lag features.

Provide insights for startups, policymakers, and infrastructure planners.

📊 Dataset

Source: Kaggle – Electric Vehicle Sales by State in India (2014–2024)

Features:

Date (month-year)

State (Indian state/UT)

Vehicle Category (2W, 3W, 4W, Bus, Others)

EV Sales Quantity

Preprocessing steps included:

Removing null/duplicate values

Standardizing state/category names

Extracting year/month

Engineering lag features and rolling averages

🔎 Methodology

Exploratory Data Analysis (EDA)

State-wise EV sales trends

Category-wise adoption (2W dominance, 3W strong in UP & Bihar)

Seasonal sales peaks (March, December)

Geographic Segmentation (Clustering)

Applied K-Means clustering on cumulative sales

Optimal clusters = 4 (Elbow Method)

Visualized via choropleth maps

Forecasting Model (XGBoost)

Features: Lagged sales, rolling averages, year/month, category encoding

Metrics:

R² = 0.64

RMSE = 0.79 (log scale)

Forecast Example: Maharashtra 2W EV sales (Jan 2025) ≈ 1083 units

📌 Results & Insights

Top states: Maharashtra, Karnataka, Tamil Nadu

Dominant category: 2-Wheelers (mass adoption driver)

Key trend: Seasonal spikes (March, December) due to policy deadlines & festivals

Cluster-based segmentation enables targeted policies & business strategies

Predictive pipeline provides actionable short-term forecasts

🛠️ Tech Stack

Python, Pandas, NumPy

Matplotlib, Seaborn, Plotly

Scikit-learn, XGBoost

Jupyter Notebook

🚀 Applications

Startups: Market entry & expansion planning

Policy Makers: Regional EV adoption strategy

OEMs & Fleet Operators: Inventory & infrastructure planning

📂 Repository Structure
├── data/                 # Raw & cleaned datasets
├── notebooks/            # Jupyter Notebooks with analysis
├── results/              # Visualizations & forecast outputs
├── EV_Geographic_Segmentation_Analysis_.ipynb
└── README.md             # Project documentation

🔮 Future Work

Integrate policy & economic factors (subsidies, fuel prices)

Extend to long-term forecasts

Build an interactive dashboard for stakeholders

👉 This project demonstrates how spatial segmentation + machine learning can guide EV adoption strategies in India.
