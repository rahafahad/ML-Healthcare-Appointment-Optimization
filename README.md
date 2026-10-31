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

<table>
  <thead>
    <tr><th>Category</th><th>Tools</th></tr>
  </thead>
  <tbody>
    <tr><td>Programming</td><td>Python</td></tr>
    <tr><td>Machine Learning</td><td>Scikit-learn, XGBoost</td></tr>
    <tr><td>Data Analysis</td><td>Pandas, NumPy</td></tr>
    <tr><td>Visualization</td><td>Matplotlib, Seaborn</td></tr>
    <tr><td>Web Application</td><td>Flask, HTML, CSS, JavaScript</td></tr>
    <tr><td>Database</td><td>SQLite</td></tr>
    <tr><td>Development</td><td>Jupyter Notebook, VS Code</td></tr>
  </tbody>
</table>

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

<table>
  <thead>
    <tr>
      <th>Metric</th>
      <th>Logistic Regression</th>
      <th>Random Forest</th>
      <th>XGBoost</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>Accuracy</td><td>67.29%</td><td>59.25%</td><td>58.68%</td></tr>
    <tr><td>Precision</td><td>32.38%</td><td>30.88%</td><td>30.69%</td></tr>
    <tr><td>Recall</td><td>56.81%</td><td>82.00%</td><td>82.98%</td></tr>
    <tr><td>F1-score</td><td>41.25%</td><td><strong>44.86%</strong></td><td>44.81%</td></tr>
    <tr><td>ROC-AUC</td><td>68.33%</td><td>73.27%</td><td><strong>73.28%</strong></td></tr>
  </tbody>
</table>

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

<pre>
ML-Healthcare-Appointment-Optimization/
├── backend/
│   ├── Intro.ipynb
│   └── ML_Models.ipynb
├── flask/
│   ├── app.py
│   └── Additional application and database scripts
├── frontend/
│   └── Frontend files
├── d3.html
├── d4.html
├── requirements.txt
└── README.md
</pre>

Run Locally

1. Clone the repository

git clone https://github.com/rahafahad/ML-Healthcare-Appointment-Optimization.git

2. Install dependencies

cd ML-Healthcare-Appointment-Optimization
pip install -r requirements.txt

3. Configure the secret key

Set the FLASK_SECRET_KEY environment variable before starting the application.

4. Start the application

cd flask
python app.py

Open the application at:

http://127.0.0.1:8000

Future Improvements

* Improve model interpretability and performance.
* Compare imbalance-handling methods under consistent conditions.
* Enhance the web interface.
* Validate models using additional datasets.

⸻

BSc (Hons) Data Science Graduation Project — University of Exeter
