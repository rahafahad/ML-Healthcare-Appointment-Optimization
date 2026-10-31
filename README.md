ML Healthcare Appointment Optimization

A machine learning project focused on predicting patient no-shows and supporting more informed medical appointment scheduling.

Overview

Missed medical appointments can affect healthcare efficiency and resource utilization. This project analyzes historical appointment data, develops machine learning models to predict no-shows, and includes a Flask web application for appointment management.

Objectives

* Explore healthcare appointment data and no-show patterns.
* Develop and compare machine learning classification models.
* Evaluate model performance using relevant metrics.
* Build a web application for patient and doctor appointment workflows.

Technologies

Category	Tools
Programming	Python
Machine Learning	Scikit-learn, XGBoost
Data Analysis	Pandas, NumPy
Visualization	Matplotlib, Seaborn
Web Application	Flask, HTML, CSS, JavaScript
Database	SQLite
Development	Jupyter Notebook, VS Code

Dataset

The dataset contains patient, medical, and appointment-related information.

Selected features: Age, Gender, Scholarship, Hypertension, Diabetes, Alcoholism, Handicap, SMS Received, Waiting Days, and Appointment Weekday.

Target — No-show:

* 0: Appointment attended
* 1: Appointment missed

Machine Learning Workflow

1. Data preprocessing and exploratory analysis
2. Feature engineering
3. Stratified train-test split
4. Class imbalance handling
5. Model training and evaluation

Model Performance

Metric	Logistic Regression	Random Forest	XGBoost
Accuracy	67.29%	59.25%	58.68%
Precision	32.38%	30.88%	30.69%
Recall	56.81%	82.00%	82.98%
F1-score	41.25%	44.86%	44.81%
ROC-AUC	68.33%	73.27%	73.28%

Key Findings

* XGBoost achieved the highest recall.
* Random Forest achieved the highest F1-score.
* Logistic Regression achieved the highest accuracy.

Note: Models used different class-imbalance handling strategies. Results are experimental and have not been clinically validated.

Web Application

The Flask application includes:

* Patient and doctor registration and login
* Appointment requests and scheduling
* Patient and doctor dashboards
* SQLite database integration

Project Structure

ML-Healthcare-Appointment-Optimization/
├── backend/
│   ├── Intro.ipynb
│   └── ML_Models.ipynb
├── flask/
│   ├── app.py
│   └── ...
├── frontend/
│   └── ...
├── d3.html
├── d4.html
├── requirements.txt
└── README.md

Run Locally

git clone https://github.com/rahafahad/ML-Healthcare-Appointment-Optimization.git
cd ML-Healthcare-Appointment-Optimization
pip install -r requirements.txt

Set the FLASK_SECRET_KEY environment variable, then run:

cd flask
python app.py

Open: http://127.0.0.1:8000

Future Improvements

* Improve model interpretability and performance.
* Compare imbalance-handling methods under consistent conditions.
* Enhance the web interface.
* Validate models using additional datasets.

⸻

BSc (Hons) Data Science Graduation Project — University of Exeter
