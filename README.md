# 🌱 NASA NDVI Vegetation Stress Classification

This project analyzes global vegetation health using NASA MODIS NDVI satellite data and applies machine learning to detect environmental stress trends.

---

## 🚀 Objective

The goal of this project is to:
- Analyze vegetation trends using NDVI (Normalized Difference Vegetation Index)
- Compare regions (Europe, Africa, Asia)
- Detect vegetation stress (declining trends)
- Apply a machine learning model to classify environmental conditions

---

## 🛰️ Data Source

- NASA MODIS Satellite Dataset  
- NDVI Product: MOD13A2  
- Provided via Google Earth Engine

---

## 🧠 Machine Learning Approach

We compute:
- Mean NDVI per region
- Temporal NDVI trend (linear slope)

Then we apply:
- Random Forest Classifier

### Labels:
- `0` → Stable / improving vegetation
- `1` → Vegetation stress (declining NDVI)

---

## 🌍 Regions Analyzed

- Europe
- Africa
- Asia

(Defined using Earth Engine bounding boxes for reproducibility)

---

## ⚙️ Tech Stack

- Python
- Google Earth Engine API
- NumPy / Pandas
- Scikit-learn
- Matplotlib

---

## 📊 Output Example

The model outputs:
- NDVI trend per region
- Classification report
- Confusion matrix
- Stress prediction for unseen values

---

## 📈 Example Insight

Regions with negative NDVI slope indicate potential:
- Deforestation
- Climate stress
- Land degradation

---

## 🧪 How to Run

1. Install dependencies:
```bash
pip install -r requirements.txt

---

## Authenticate Earth Engine:

ee.Authenticate()
Run the Colab notebook or Python script

---

## 📦 Requirements
See requirements.txt

---

## 👨‍💻 Author

Angelo Sorte

---

## 🌱 Future Improvements
Pixel-level NDVI heatmaps
Time-series deep learning (LSTM)
Global vegetation anomaly detection
Interactive Earth Engine dashboard
