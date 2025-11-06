WealthWise: Smart Financial Planner & Analyzer 🧠💰

🚀 Project Overview
WealthWise is an integrated web application designed to empower users with data-driven financial insights and predictive intelligence. It features multiple machine learning models to analyze personal financial data, recommend optimal investment allocations, forecast asset growth, and determine retirement readiness.

The application is built on Flask for a smooth web experience and leverages key datasets for training and demonstration purposes, providing a powerful, interactive dashboard for smarter financial decision-making.

✨ Key Features
The application provides the following core tools:

1.	📊 Asset Growth Predictor:

Predicts the future value of an investment (Lumpsum or SIP) based on initial amount, contributions, return rate, and time horizon.
Features a line chart visualization of the projected growth over the specified years.

2.	💰 Expenses & Savings Visualizer:

Allows users to input categorized expenses and total income to calculate and visualize Net Savings.

3.	📈 Investment Pathway Allocator:

A machine learning model (trained on f2investmentPathway.csv) recommends a balanced portfolio allocation (Equity, Debt, Gold, Real Estate) based on the user's Age, Risk Score, and Time Horizon.
The recommended allocation is displayed with a Doughnut Chart.

4.	👵 Retirement Readiness Analyzer:

Predicts a user's Retirement Readiness Score (0-100) using inputs like Age, Income, Expenses, Investment, Inflation, and Expected Return Rate.
Provides clear status and a colored progress bar (e.g., Green for Excellent, Red for Needs Attention).

💻 Tech Stack & Dependencies

•	Backend Framework: Python 3.x, Flask

•	Machine Learning/Data Science: scikit-learn, joblib, pandas, numpy

•	Database: sqlite3 (Used for basic data persistence, e.g., in test_app2 (1).py)

•	Frontend: HTML5, CSS3, Jinja Templating, Bootstrap

•	Visualization: Chart.js
