# Job-Acceptance-Prediction-System
An end-to-end HR Analytics &amp; Machine Learning project that predicts whether a candidate will accept or reject a job offer, helping HR teams reduce offer dropouts and optimize recruitment decisions.
📌 Problem Statement

Recruitment teams deal with thousands of candidates, but not all offered candidates accept the job.
Offer rejections lead to:

Increased hiring cost

Longer hiring cycles

Resource wastage

This project builds a Job Acceptance Prediction System that:

Predicts job acceptance probability

Identifies high-risk dropout candidates

Provides actionable insights to HR teams

🧠 Business Use Cases

Predict candidate offer acceptance before releasing offers

Reduce offer dropouts

Optimize interview & evaluation strategies

Support data-driven HR decisions

Identify high-risk candidates early

📊 Dataset Overview

Total Records: ~50,000
Domain: HR Analytics / Recruitment

Key Features

Academic Performance (SSC, HSC, Degree)

Interview Scores (Technical, Aptitude, Communication)

Skills Match Percentage

Experience & Employment Gap

CTC Expectation Gap

Company Tier & Competition Level

Candidate Preferences (Relocation, Bond, Career Switch)

Target Variable:

job_acceptance_status

1 → Accepted

0 → Rejected

🏗️ Project Architecture
Data Collection
      ↓
Data Cleaning & Validation
      ↓
Feature Engineering
      ↓
Machine Learning Model (Random Forest)
      ↓
Prediction Probability
      ↓
Streamlit Dashboard (HR View)

⚙️ Tech Stack

Programming: Python

Data Analysis: Pandas, NumPy

Machine Learning: Scikit-Learn

Visualization & UI: Streamlit

Modeling: Random Forest Classifier

Deployment: Local / Cloud Ready

🔍 Data Preprocessing Highlights

✔ Column normalization
✔ String → Numeric conversion
✔ Missing value handling
✔ Logical range validation
✔ Categorical encoding
✔ Schema validation

Designed to handle real-world noisy HR data

🧪 Feature Engineering

Academic Score (weighted SSC, HSC, Degree)

Interview Performance Score

CTC Expectation Gap

Experience Category

Offer Dropout Risk Score

These features improve business relevance, not just accuracy.

🤖 Machine Learning Model

Algorithm: Random Forest Classifier

Class Imbalance Handling: class_weight="balanced"

Business Threshold: 0.40 (instead of default 0.50)

Evaluation Metrics:

Precision

Recall

F1-Score

The model is intentionally conservative to flag rejection risk early.

📈 Streamlit Dashboard Features

HR-friendly UI

Real-time prediction

Acceptance & rejection probabilities

Business-driven thresholds

KPI metrics:

Acceptance Rate

Dropout Rate

Skills Match Average

▶️ How to Run the Project
1️⃣ Clone the Repository
git clone https://github.com/your-username/job-acceptance-prediction-system.git
cd job-acceptance-prediction-system

2️⃣ Create Virtual Environment
python -m venv venv
venv\Scripts\activate

3️⃣ Install Dependencies
pip install -r requirements.txt

4️⃣ Run Data Pipeline
python run_pipeline.py

5️⃣ Train Model
python train.py

6️⃣ Launch Streamlit App
python -m streamlit run app.py
