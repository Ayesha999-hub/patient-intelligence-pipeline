#  Patient Intelligence Pipeline  
### Mining Temporal Patterns & Building Predictive Models on Patient Vital Data

This project implements a complete **data mining and machine learning pipeline** for analyzing patient vital signs and predicting clinical conditions using time series analysis, similarity search, and supervised classification.

---

##  Overview

Healthcare systems collect continuous patient data but often lack actionable insights.

This project addresses that gap by building a pipeline that can:

-  Analyze temporal trends in patient vitals  
-  Detect anomalies in physiological signals  
-  Identify clinically similar patients  
-  Predict patient diagnoses using machine learning  

The work simulates a **real-world clinical decision support system**.

---

## 📊 Dataset

- **Type:** Simulated Patient Vitals Dataset  
- **Size:** ~60,000 records  
- **Patients:** 500  
- **Time Span:** 30 days (6-hour intervals)  

### Features include:
- Heart Rate  
- Blood Pressure (Systolic & Diastolic)  
- Blood Oxygen Level (SpO2)  
- Body Temperature  
- Respiratory Rate  
- Sleep Hours  
- Stress Level  
- Demographics (Age, Gender)  
- Diagnosis (Target Variable)

---

## ⚙️ Pipeline Architecture

### 1️⃣ Data Preprocessing
- Data cleaning and validation  
- Physiological range filtering  
- Time-series structuring  
- Feature engineering (mean, std, min, max, trend)

---

### 2️⃣ Time Series Analysis
- Visualization of patient vitals  
- Rolling averages (7 & 14 windows)  
- Time series decomposition  
- Anomaly detection using statistical thresholds  

---

### 3️⃣ Similarity Search
- Euclidean & Manhattan distance comparison  
- Dynamic Time Warping (DTW) for time-series similarity  
- Patient matching for clinical decision support  

---

### 4️⃣ Machine Learning Models

The following classifiers were implemented and compared:

- 🌳 Decision Tree  
- 📜 Rule-Based Classification  
- 📍 k-Nearest Neighbors (kNN)  
- 📊 Naïve Bayes  
- ⚡ Support Vector Machine (SVM)  

Each model was evaluated using:
- Accuracy  
- Precision  
- Recall  
- F1-score  
- Confusion Matrix  

---

## 📈 Key Results

- Strong separation between diagnosis classes  
- High anomaly rates observed in Arrhythmia patients  
- Distance-based methods effectively grouped similar patients  
- All classifiers achieved very high accuracy (dataset is highly structured)

⚠️ Note: Extremely high accuracy may indicate strong feature separability or potential overfitting.

---

## 🧠 Clinical Insights

- Irregular heart rate patterns strongly indicate **Arrhythmia**  
- Elevated blood pressure correlates with **Hypertension**  
- Low sleep duration is a key indicator of **Sleep Disorders**  
- Time-series analysis reveals patterns not visible in summary statistics  

---

## 🛠️ Tech Stack

- **Python**
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn  
- Statsmodels  
- tslearn / dtaidistance  

---

## 📂 Project Structure

---

## 🚀 How to Run

1. Clone the repository:
```bash
git clone https://github.com/yourusername/patient-intelligence-pipeline.git
2. Open in Google Colab or Jupyter Notebook
3. Install dependencies:
pip install -r requirements.txt
4. Run the notebook step by step
Applications
Clinical decision support systems
Remote patient monitoring
Early detection of health deterioration
Personalized healthcare analytics
📌 Future Improvements
Use real-world clinical datasets
Add deep learning models (LSTM for time series)
Deploy as a real-time monitoring dashboard
Improve interpretability with explainable AI (XAI)

