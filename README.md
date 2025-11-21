🩺 MediTrack Health —Analysis

A streamlined, AI-powered health risk screening system designed with a professional interface, focusing on clarity, accuracy, and medical-grade usability.
MediTrack evaluates early risks for Diabetes, Breast Cancer, Heart Disease, and Kidney Disease using machine learning models stored in the artifacts/ directory.

🛡️ Project Badges

<p align="center"><img src="https://img.shields.io/badge/Mode-Dark%20Theme-000000?style=for-the-badge"/>  
<img src="https://img.shields.io/badge/Framework-Streamlit-111111?style=for-the-badge&logo=streamlit&logoColor=red"/>  
<img src="https://img.shields.io/badge/AI%20Models-4%20Integrated-222222?style=for-the-badge"/>  
<img src="https://img.shields.io/badge/Python-3.10+-333333?style=for-the-badge&logo=python"/>  
<img src="https://img.shields.io/badge/Status-Stable-181818?style=for-the-badge"/>  </p>
---

1. Overview

MediTrack Health is a single-screen, real-time screening interface that provides AI-driven probability scores for four major diseases. The dark theme improves focus, reduces visual noise, and presents a more modern clinical dashboard experience.

2. Supported Disease Models

MediTrack provides early-risk probabilities for:

Diabetes

Heart Disease

Breast Cancer

Kidney Disease


Each prediction includes:

Score Range	Category	Indicator Color

0–40%	Low Risk	#00ff9d (Neon Green)
40–70%	Moderate Risk	#ffed4a (Neon Yellow)
70–100%	High Risk	#ff3b4e (Neon Red)

3. User Interface (Dark Mode Layout)

══════════════════════════════════════════════════════════════
   MED ITRACK HEALTH  |  AI RISK SCREENING INTERFACE (DARK)
══════════════════════════════════════════════════════════════

 Disease Model: [ Diabetes ▼ ]

 • Full Name: __________________________
 • Age: ______      • BMI: _______
 • Glucose: _______ • Blood Pressure: ______
 • Heart Rate: _____• Temperature: ________

 [ ] I confirm that all data entered is accurate.

                   [ Run Prediction ]

══════════════════════════════════════════════════════════════
 Result: HIGH RISK (82%)   •   Status: Immediate Evaluation
══════════════════════════════════════════════════════════════

4. Installation

pip install -r requirements.txt
streamlit run app.py

System initializes:

[Loading Models...] ███████████████ 100%
[Launching Dark UI...] ███████████████ 100%
[Ready on] → http://localhost:8501


---

5. System Architecture

User Inputs
     ↓
Validation Layer
     ↓
Preprocessing (Scaling + Numerical Encoding)
     ↓
ML Model from /artifacts
     ↓
Probability Output
     ↓
Risk Categorization (Color-coded)
     ↓
User Display

6. Machine Learning Pipeline

Preprocessing

Standardized numerical features

Strict data validation

Feature vector assembly


Models Utilized

(Reflects typical clinical ML workflows; can be updated to match your actual training.)

Logistic Regression

Random Forest Classifier

Support Vector Classifier

Gradient Boosting


Risk Classification

Models output a probability which is mapped into defined medical risk tiers.


7. Project Structure

MediTrack-Health/
│── app.py
│── artifacts/
│    ├── diabetes.pkl
│    ├── breast_cancer.pkl
│    ├── heart.pkl
│    └── kidney.pkl
│── static/
│    └── dark-medical-logo.png
│── requirements.txt
└── README.md


---

8. Future Enhancements

Add liver disease and anemia predictors

Generate downloadable dark PDF reports

Add multi-disease comparison dashboard

Add mobile-optimized dark UI

Multi-language support



---

9. Author

Uneeba Nadeem
AI • Machine Learning • Data Science


---
