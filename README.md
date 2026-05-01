# Composite Behavioral Modeling for Identity Theft Detection 🛡️

**A sophisticated Cybersecurity-focused Machine Learning platform designed to detect identity theft in Online Social Networks (OSNs) through ensemble behavioral analysis.**

[![Tech Stack](https://img.shields.io/badge/Stack-Python%20|%20Flask%20|%20ML-blue)](#technical-stack)

---

## ✨ Project Overview
This platform utilizes a **compositive behavioral modeling** approach, integrating multiple machine learning classifiers to identify fraudulent user patterns. By analyzing digital interactions and transactional data, the system distinguishes between genuine users and impersonators with high precision.

---

## 🚀 Key Modules

### 👨‍💼 Admin Module
*   **Dataset Lifecycle Management:** Facilities for secure uploading and viewing of social network interaction datasets.
*   **Preprocessing Engine:** Automated data cleaning, feature selection (dropping non-predictive IDs), and label encoding for categorical behavioral data.
*   **Ensemble Model Execution:** Parallel execution of multiple classifiers:
    *   **Support Vector Machine (SVM):** For high-dimensional boundary classification.
    *   **Random Forest:** For robust, non-linear decision making via bagging.
    *   **Decision Tree:** For clear, interpretable behavioral logic.
*   **Performance Analytics:** Real-time generation of accuracy comparison graphs using **Matplotlib** to identify the most effective detection model.

### 👤 User Module
*   **Behavioral Visualization:** Graphical classification of contract types and user interaction patterns.
*   **Real-Time Detection:** A predictive interface where users can input behavioral parameters to receive an immediate "Theft" or "No Theft" risk assessment.

---

## 🛠️ Technical Stack
*   **Backend:** Python, Flask Framework.
*   **Machine Learning:** Scikit-learn, Joblib (Model Serialization), Pandas (Data Manipulation).
*   **Database:** SQLite3 (User Authentication & Metadata).
*   **Visualization:** Matplotlib (Agg backend for server-side plot generation).
*   **Frontend:** HTML5, CSS3, Jinja2 Templating.

---

## ⚙️ Engineering Highlights
*   **Hybrid Classification:** Improves detection reliability by comparing SVM, Random Forest, and Decision Tree results, reducing false positives common in single-model systems.
*   **Persistence Layer:** Models are trained once and serialized using **Joblib**, allowing for high-speed inference without retraining during the detection phase.
*   **Relational Security:** Implements a localized **SQLite** database for secure user registration and session-based authentication.

---

## 🚀 Getting Started
1. **Clone the repo:** `git clone https://github.com/angalagouthamkumar/Identity-Theft-Detection.git`
2. **Install dependencies:** `pip install flask pandas scikit-learn xlrd joblib matplotlib`
3. **Run the app:** `python3 App.py`
