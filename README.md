💡 WealthWise: Smart Financial Planner & Analyzer 🧠💰
🚀 Project Overview
WealthWise is an intelligent web application that empowers users with data-driven financial insights and predictive analytics.
Built with Python (Flask) and multiple machine learning models, it helps users analyze their finances, forecast investments, and plan for retirement — all through an interactive and intuitive dashboard.
The system uses real and synthetic datasets for model training and offers comprehensive tools for smarter financial decision-making.
________________________________________
✨ Key Features
1. 📊 Asset Growth Predictor
•	Predicts the future value of investments (Lumpsum or SIP) based on:
o	Initial amount
o	Monthly contribution
o	Expected return rate
o	Investment duration
•	Displays line chart visualization of projected growth over time.
2. 💰 Expenses & Savings Visualizer
•	Accepts categorized expense inputs and total income.
•	Calculates and visualizes Net Savings using interactive charts.
3. 📈 Investment Pathway Allocator
•	A machine learning model trained on f2investmentPathway.csv recommends a balanced investment portfolio (Equity, Debt, Gold, Real Estate).
•	Inputs: Age, Risk Score, Time Horizon
•	Output: Recommended allocation shown via Doughnut Chart.
4. 👵 Retirement Readiness Analyzer
•	Predicts a Retirement Readiness Score (0-100) using:
o	Age
o	Income
o	Expenses
o	Current Investments
o	Inflation & Expected Return Rate
•	Displays a colored progress bar (Green → Excellent, Red → Needs Attention).
________________________________________
💻 Tech Stack
Category	Tools / Libraries
Backend	Python 3.x, Flask
Machine Learning / Data Science	scikit-learn, pandas, numpy, joblib
Database	SQLite3 (basic data persistence)
Frontend	HTML5, CSS3, Bootstrap, Jinja2
Visualization	Chart.js
________________________________________
🛠️ Installation & Setup
Prerequisites
•	Python 3.8+
•	Git
Steps
1.	Clone the Repository
2.	git clone [YOUR_REPOSITORY_URL]
3.	cd [your-project-folder]
4.	Create and Activate Virtual Environment
5.	python -m venv venv
6.	# macOS/Linux:
7.	# source venv/bin/activate
8.	# Windows:
9.	# venv\Scripts\activate
10.	Install Dependencies
11.	pip install Flask joblib numpy pandas scikit-learn
12.	Train and Save Models
Before running the app, train and save models in the models/ directory (as referenced in app.py).
13.	mkdir models
14.	python train_asset_growth_model.py
This script trains a DecisionTreeRegressor for asset growth prediction and saves it as a .pkl file in the models/ folder.
Ensure you also have .pkl models for:
o	Investment Pathway (f2investmentPathway.pkl)
o	Expenses & Savings
o	Retirement Readiness (retirement_readiness_model_optimized.pkl)
15.	Run the Application
16.	python app.py
17.	Open in Browser
Visit: http://127.0.0.1:5000/
________________________________________
📂 Project Structure
🧠 Application Files
File	Description
app.py	Main Flask app — handles routes, templates, and model predictions.
test_app2 (1).py	Development/test Flask app with SQLite setup for retirement data.
train_asset_growth_model.py	Script that trains and saves the Asset Growth Prediction model.
________________________________________
📈 Data Files
File	Description	Used In
asset_growth_data.csv	Synthetic dataset for predicting investment growth.	Asset Growth Predictor
f1_financial_profiles.csv	General demographic & financial metrics.	Multiple features
f2investmentPathway.csv	Portfolio allocation dataset based on risk & time horizon.	Investment Allocator
feature3_expense_dataset (1).csv	Categorized expenses and income data.	Expenses & Savings
retirement_readiness_data.csv	Financial inputs with readiness scores.	Retirement Analyzer
________________________________________
🌐 Frontend Templates
File	Description
index.html	Landing page introducing WealthWise.
dashboard.html	Main navigation hub linking all prediction tools.
asset_growth.html	Input form & chart for Asset Growth Predictor.
expenses_savings.html	Inputs & visualization for Expenses & Savings.
investment_path.html	Inputs & Doughnut Chart for portfolio allocation.
retirement_readiness.html	Inputs & progress bar for Readiness Score.
________________________________________
📜 Summary
WealthWise combines machine learning, data visualization, and financial modeling into one intelligent, interactive platform — helping users make smarter financial decisions with predictive confidence.
💬 “Your money should work for you — not the other way around.”


