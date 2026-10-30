ML Healthcare Appointment Optimization

A Machine Learning-based healthcare project focused on predicting patient no-shows and supporting more informed medical appointment scheduling.

Project Overview

Missed medical appointments can affect healthcare resource utilization, increase waiting times, and reduce scheduling efficiency.

This project investigates how Machine Learning techniques can identify patients who are more likely to miss their scheduled appointments using historical appointment data.

It also includes a Flask-based web application for patient and doctor appointment management workflows.

Project Objectives

* Analyze historical healthcare appointment data.
* Explore factors associated with patient no-shows.
* Develop Machine Learning classification models.
* Evaluate and compare model performance.
* Build a web application to support appointment-related workflows.

Technologies & Tools

* Programming Language: Python
* Machine Learning: Scikit-learn, XGBoost
* Data Analysis: Pandas, NumPy
* Data Visualization: Matplotlib, Seaborn
* Web Framework: Flask
* Database: SQLite
* Frontend: HTML, CSS, JavaScript
* Development Tools: Jupyter Notebook, VS Code

Dataset & Features

The project uses historical medical appointment data containing patient and appointment-related information.

The analysis includes features such as:

* Age
* Gender
* Scholarship status
* Hypertension
* Diabetes
* Alcoholism
* Handicap status
* SMS notifications
* Waiting days
* Appointment weekday

Target variable: No-show

* 0: Patient attended the appointment.
* 1: Patient did not attend the appointment.

Machine Learning Workflow

1. Data Preprocessing: Cleaning and preparing the dataset.
2. Exploratory Data Analysis: Examining patient characteristics and appointment attendance patterns.
3. Feature Engineering: Creating features such as waiting days and appointment weekdays.
4. Data Splitting: Using stratified training and testing sets.
5. Class Imbalance Handling: Applying SMOTE for selected models and class weighting for XGBoost.
6. Model Training: Training three classification algorithms.
7. Model Evaluation: Comparing models using accuracy, precision, recall, F1-score, and ROC-AUC.

Machine Learning Models & Results

The following models were evaluated:

| Metric | Logistic Regression | Random Forest | XGBoost |
| --- | --- | --- | --- |
| Accuracy | 67.29% | 59.25% | 58.68% |
| Precision | 32.38% | 30.88% | 30.69% |
| Recall | 56.81% | 82.00% | 82.98% |
| F1-score | 41.25% | **44.86%** | 44.81% |
| ROC-AUC | 68.33% | 73.27% | **73.28%** |

Key Findings

* XGBoost achieved the highest recall at 82.98%.
* Random Forest achieved the highest F1-score at 44.86%.
* Logistic Regression achieved the highest accuracy at 67.29%.
* XGBoost and Random Forest achieved very similar ROC-AUC scores.

The results demonstrate the importance of selecting evaluation metrics according to the intended prediction objective, particularly when identifying potential patient no-shows.

Note: The models used different class-imbalance handling strategies, so their results should be interpreted with this methodological difference in mind. These are experimental results and have not been clinically validated.

Web Application

The project includes a Flask-based web application with appointment-related functionality, including:

* Patient and doctor registration and login.
* Appointment request workflows.
* Appointment scheduling.
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
│   ├── appointdbscript.py
│   ├── logindbscript.py
│   └── ...
│
├── frontend/
│   └── ...
│
├── d3.html
├── d4.html
├── requirements.txt
└── README.md

Directory Overview

* backend/ – Data exploration, preprocessing, feature engineering, and machine learning experiments.
* flask/ – Flask application and database-related scripts.
* frontend/ – Frontend files for the web application.
* d3.html / d4.html – Additional project interface or visualization files.
* requirements.txt – Python dependencies required to run the project.
* README.md – Project documentation and setup instructions.

Running the Project Locally

1. Clone the repository

git clone https://github.com/rahafahad/ML-Healthcare-Appointment-Optimization.git

2. Navigate to the project

cd ML-Healthcare-Appointment-Optimization

3. Install dependencies

pip install -r requirements.txt

4. Configure the environment variable

Set a securely generated environment variable named FLASK_SECRET_KEY before running the application.

Never commit secret keys or credentials to the repository.

5. Run the application

cd flask
python app.py

Open your browser at:

http://127.0.0.1:8000

Future Improvements

* Further optimize model performance.
* Improve model interpretability.
* Compare class-imbalance handling strategies under consistent experimental conditions.
* Enhance the web application interface.
* Validate model performance on additional datasets before real-world deployment.

⸻

Developed as a BSc (Hons) Data Science graduation project at the University of Exeter.
