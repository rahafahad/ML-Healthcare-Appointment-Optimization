ML Healthcare Appointment Optimization

A machine learning-based healthcare project that explores patient no-show prediction and supports more informed medical appointment scheduling.

Project Overview

Missed medical appointments can reduce healthcare resource utilization, increase waiting times, and affect scheduling efficiency.

This project uses historical medical appointment data to investigate patterns associated with patient no-shows and develop machine learning models to predict the likelihood of missed appointments.

It also includes a Flask-based web application that supports patient and doctor appointment management workflows.

Project Objectives

* Analyze historical healthcare appointment data.
* Identify factors associated with patient no-shows.
* Develop and evaluate machine learning classification models.
* Compare model performance using multiple evaluation metrics.
* Build a web application for appointment-related workflows.


Table Test

Model	Accuracy
Logistic Regression	67.29%
Random Forest	59.25%
XGBoost	58.68%

Technologies & Tools

Category	Technologies
Programming Language	Python
Machine Learning	Scikit-learn, XGBoost
Data Analysis	Pandas, NumPy
Data Visualization	Matplotlib, Seaborn
Web Framework	Flask
Database	SQLite
Frontend	HTML, CSS, JavaScript
Development Tools	Jupyter Notebook, VS Code

Machine Learning Models & Results

Metric	Logistic Regression	Random Forest	XGBoost
Accuracy	67.29%	59.25%	58.68%
Precision	32.38%	30.88%	30.69%
Recall	56.81%	82.00%	82.98%
F1-score	41.25%	44.86%	44.81%
ROC-AUC	68.33%	73.27%	73.28%
Dataset & Features

The project uses historical medical appointment data containing patient demographics, medical conditions, and appointment information.

The dataset includes features such as:

* Age and gender
* Scholarship status
* Hypertension and diabetes
* Alcoholism and handicap status
* SMS notifications
* Waiting days
* Appointment weekday

Target variable: No-show

* 0: Patient attended the appointment.
* 1: Patient did not attend the appointment.

Machine Learning Workflow

1. Data Preprocessing: Cleaning and preparing the dataset.
2. Exploratory Data Analysis: Investigating patterns and relationships in the data.
3. Feature Engineering: Creating features such as waiting days and appointment weekdays.
4. Data Splitting: Creating stratified training and testing sets.
5. Class Imbalance Handling: Applying SMOTE to selected models and class weighting for XGBoost.
6. Model Training: Training three classification algorithms.
7. Model Evaluation: Comparing performance using accuracy, precision, recall, F1-score, and ROC-AUC.

Machine Learning Models & Results

Three classification models were evaluated:

Metric	Logistic Regression	Random Forest	XGBoost
Accuracy	67.29%	59.25%	58.68%
Precision	32.38%	30.88%	30.69%
Recall	56.81%	82.00%	82.98%
F1-score	41.25%	44.86%	44.81%
ROC-AUC	68.33%	73.27%	73.28%

Key Findings

* XGBoost achieved the highest recall (82.98%), identifying the largest proportion of actual no-show cases.
* Random Forest achieved the highest F1-score (44.86%).
* Logistic Regression achieved the highest accuracy (67.29%).
* Random Forest and XGBoost achieved nearly identical ROC-AUC scores.

The findings highlight the importance of selecting evaluation metrics according to the prediction objective, especially when identifying potential patient no-shows.

Evaluation note: The models used different class-imbalance handling strategies, so their results should be interpreted with this methodological difference in mind. These results are experimental and have not been clinically validated.

Web Application

The project also includes a Flask-based web application with the following functionality:

* Patient and doctor registration and login.
* Appointment request and scheduling workflows.
* Patient and doctor dashboards.
* SQLite database integration.

Project Structure

ML-Healthcare-Appointment-Optimization/
│
├── backend/
│   ├── Intro.ipynb
│   └── ML_Models.ipynb
│
├── flask/
│   ├── app.py
│   └── ...
│
├── frontend/
│   └── ...
│
├── d3.html
├── d4.html
├── requirements.txt
└── README.md

Running the Project Locally

1. Clone the repository

git clone https://github.com/rahafahad/ML-Healthcare-Appointment-Optimization.git

2. Navigate to the project directory

cd ML-Healthcare-Appointment-Optimization

3. Install dependencies

pip install -r requirements.txt

4. Configure the Flask secret key

Set an environment variable named FLASK_SECRET_KEY using a securely generated secret key before starting the application.

Never commit secret keys or credentials to the repository.

5. Run the application

cd flask
python app.py

Open the application in your browser:

http://127.0.0.1:8000

Future Improvements

* Further optimize and evaluate model performance.
* Improve model interpretability.
* Compare class-imbalance handling strategies under consistent experimental conditions.
* Enhance the web application interface.
* Validate model performance using additional datasets before considering real-world deployment.

⸻

Developed as a BSc (Hons) Data Science graduation project at the University of Exeter.
