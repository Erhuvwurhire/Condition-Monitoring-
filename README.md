# Condition-Monitoring-
AI-Based Condition Monitoring of Industrial Equipment Using Vibration and Temperature Data
# 🔧 AI-Based Condition Monitoring System

> End-to-end Industrial AI project for detecting anomalies and monitoring the health of industrial machinery using real-time vibration and temperature data.

---

## 🚀 Overview

This project implements a condition monitoring system that applies machine learning techniques to time-series sensor data ( vibration, temperature, pressure) for early fault detection and maintenance planning.

Using open-source datasets and real-world engineering principles, the system demonstrates how to:
- Extract meaningful features from raw sensor data
- Detect early-stage equipment faults and anomalies
- Deploy a real-time monitoring dashboard for operators
- Simulate MLOps-ready deployment pipelines using Docker

---

## 🧠 Use Cases

- Predictive maintenance for rotating machinery (motors, turbines, bearings)
- Anomaly detection in aerospace components
- Intelligent alerting in manufacturing environments

---

## 📊 Key Features

✅ FFT and statistical signal analysis  
✅ Fault classification and anomaly detection (ML + DL models)  
✅ Rolling window feature extraction  
✅ Real-time dashboard with alert flags  
✅ Fully containerized with Docker  
✅ Compatible with edge/cloud simulation  

---

## 🧰 Tech Stack

| Category             | Tools / Libraries                                                                 |
|----------------------|------------------------------------------------------------------------------------|
| Programming Language | Python                                                                             |
| ML/DL Frameworks     | Scikit-learn, PyTorch, XGBoost, Autoencoders                                       |
| Signal Processing    | SciPy, NumPy, Pandas                                                               |
| Visualization        | Matplotlib, Seaborn, Plotly, Streamlit                                             |
| Deployment           | Docker, FastAPI (optional), Streamlit                                              |
| Workflow             | Git, GitHub Actions, Jupyter Notebooks                                             |
| Data Sources         | [CWRU Bearing Dataset](https://engineering.case.edu/bearingdatacenter), NASA CMAPSS|

---

## 🗃 Project Structure
condition-monitoring-ai/
├── data/ # Raw and preprocessed sensor data
├── notebooks/ # EDA and modeling notebooks
├── src/ # Source code (training, feature extraction)
│ ├── preprocessing.py
│ ├── train_model.py
│ ├── predict.py
│ └── utils.py
├── app/ # Streamlit dashboard
│ └── dashboard.py
├── Dockerfile # Container spec
├── requirements.txt
├── README.md
└── LICENSE


---

## ⚙️ How It Works

1. **Data Loading**: Import vibration or temperature sensor data.
2. **Signal Processing**: Apply FFT, rolling stats, and domain-specific transforms.
3. **Feature Extraction**: Compute time-frequency features like RMS, skewness, spectral entropy.
4. **Model Training**:
   - Supervised classification (Random Forest, CNN)
   - Unsupervised anomaly detection (Autoencoder, Isolation Forest)
5. **Deployment**:
   - Real-time dashboard using Streamlit
   - Docker container for easy portability

---

## 💻 Quick Start

### 🔨 Local Setup

```bash
# Clone the repo
git clone https://github.com/yourusername/condition-monitoring-ai.git
cd condition-monitoring-ai

## Create a virtual environment
python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate

## Install dependencies
pip install -r requirements.txt

cd app
streamlit run dashboard.py

---


🧪 Example Results

Model	Accuracy	Precision	F1-score
RandomForest	91.2%	90.4%	90.8%
LSTM Autoencoder	—	—	AUC-ROC: 0.94

 📚 References

Case Western Reserve Bearing Data Center

NASA CMAPSS Turbofan Engine Dataset

ISO 10816 Machine Vibration Standards

"A Review of Deep Learning Techniques for Condition Monitoring" – IEEE

 📈 Future Improvements

Add support for streaming data via MQTT or Kafka

Deploy model via REST API with FastAPI or Flask

Incorporate transformer-based models for complex sequences

Integrate LangChain + vector DB for fault documentation search


