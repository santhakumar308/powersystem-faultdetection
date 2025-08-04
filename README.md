# 🔌 Power System Fault Detection and Classification using Machine Learning

## 📌 Project Overview

This project aims to build a machine learning model that classifies different types of faults in a power distribution system using both **electrical parameters** (such as voltage, current, and power) and **environmental conditions** (like temperature, wind, and weather status).

The model was developed, trained, and evaluated using **IBM Watson Studio** (Lite Plan) and a real-world fault dataset sourced from [Kaggle](https://www.kaggle.com/datasets/ziya07/power-system-faults-dataset).

---

## 🎯 Objective

To classify power system faults into categories such as:
- **Line Break**
- **Transformer Fault**
- **Overheating**

using features like:
- Voltage (V)
- Current (A)
- Power Load (MW)
- Temperature (°C)
- Wind Speed
- Weather Condition
- Maintenance Status
- Component Condition
- Duration and Downtime

---

## 🧠 ML Approach

### 🔎 Data Preprocessing
- Label Encoding for categorical columns (`Weather`, `Maintenance`, `Component`)
- Normalization of numerical columns (`Voltage`, `Current`, etc.)
- Splitting into training (80%) and testing (20%) datasets

### ⚙️ Model
- **Algorithm Used:** Random Forest Classifier
- **Reason:** Handles mixed data types and provides high accuracy with interpretability

### 🧪 Evaluation
- Accuracy Score
- Confusion Matrix
- Precision & Recall metrics

### ✅ Achieved Accuracy: ~93%

## 📊 Sample Input and Prediction

**Input Features:**  
```json
{
  "Voltage": 1500,
  "Current": 150,
  "Power Load": 50,
  "Temperature": 25,
  "Wind Speed": 20,
  "Weather": "Clear",
  "Maintenance": "Scheduled",
  "Component": "Normal"
}
