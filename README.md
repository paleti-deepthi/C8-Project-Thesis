# 🌍 Air-O-Health: AQI Prediction & Health Advisory System

## 👩‍💻 Authors
- P. Deepthi (Y22ACS519)  
- K. Vara Brahma Reddy (Y22ACS486)  
- Maha Lakshmi N T (Y22ACS494)  
- P. Bharadwaj (Y22ACS521)  

---

## 📌 Overview
**Air-O-Health** is a dual-engine air quality monitoring and prediction system designed to provide **real-time AQI insights and future forecasts** for major Indian cities.

The platform integrates:
- 🌐 **Live AQI Monitoring (WAQI API)**
- 🤖 **Machine Learning-based AQI Forecasting**
- 🩺 **Health Risk Advisory System**
- 📊 **Interactive Web Dashboard**
- 🤖 **AI Chatbot (AirBot)**

It enables users to understand air quality conditions and take **preventive health measures** effectively.

---

## ⚙️ Project Components

### 1. Live AQI Engine
- Fetches real-time data from WAQI API  
- Converts AQI between **US-EPA** and **India-NAQI** standards  
- Implements **10-minute caching** for performance optimization  

---

### 2. Forecast Engine (ML Model)
- Ensemble model using:
  - Random Forest  
  - XGBoost  
- Predicts AQI for future dates  
- Uses **city-month historical statistics**  
- Achieves **98.16% accuracy (R² Score)**  

---

### 3. Health Advisory System
- Maps AQI values to health categories  
- Generates:
  - Pollution causes  
  - Health precautions  
- Supports dual standards:
  - US-EPA  
  - India-NAQI  

---

### 4. Web Dashboard
- Built using HTML, Tailwind CSS, and JavaScript  
- Features:
  - 📊 Pollutant charts (Chart.js)  
  - 🗺️ Interactive map (Leaflet.js)  
  - 🌈 Dynamic AQI-based UI  
  - 📄 PDF report export  

---

### 5. AirBot Chatbot
- Provides instant responses to:
  - AQI queries  
  - Pollutant information  
  - Health guidance  
- Context-aware assistant integrated into UI  

---

## 🏗️ System Architecture
The system follows a **3-tier architecture**:

- **Frontend Layer** → Interactive Dashboard (HTML, Tailwind, JS)  
- **Backend Layer** → FastAPI Server  
- **Data & Model Layer** → ML Models + Dataset  

### Workflow:
1. User selects city, mode, and standard  
2. Request sent to FastAPI backend  
3. Either:
   - Live data fetched via API  
   - OR prediction generated via ML model  
4. AQI + health advisory returned to frontend  
5. Dashboard updates dynamically  

---

## 🧠 Technologies Used

### Backend
- Python  
- FastAPI  
- Scikit-learn  
- XGBoost  
- Joblib  
- Requests  

### Frontend
- HTML5  
- Tailwind CSS  
- JavaScript  
- Chart.js  
- Leaflet.js  

### Data & Tools
- Pandas  
- NumPy  
- Matplotlib  

### APIs & Services
- WAQI API (World Air Quality Index)  

---

## 📊 Model Performance

| Model            | Accuracy (R² Score) |
|------------------|-------------------|
| Random Forest    | 93.77%            |
| XGBoost          | 99.85%            |
| **Overall Model**| **98.16%**        |

---

## ✨ Key Features
- 🌐 Real-time AQI monitoring  
- 🔮 Future AQI prediction  
- 🔁 Dual AQI standard support  
- 📊 Interactive visualization dashboard  
- 🧠 AI-powered chatbot  
- 📄 PDF report generation  
- ⚡ Fast API with caching  
- 🗺️ Location-based map visualization  

---

## 🚀 Installation & Setup

### 1. Clone Repository
```bash
git clone https://github.com/your-username/air-o-health.git
cd air-o-health
