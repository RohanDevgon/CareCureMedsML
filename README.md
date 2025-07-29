# 💊 CareCureMeds: Disease Prediction and Hospital Locator System

**CareCureMeds** is a machine learning-powered web application that predicts diseases based on symptoms and locates nearby hospitals based on the predicted condition. It combines intelligent diagnosis, interactive visualizations, and map-based hospital ratings to assist users in health decision-making.

---

## 🌟 Features

- ✅ **Symptom-based Disease Prediction**
- 📍 **Map Visualization of Hospitals Based on Ratings**
- 📊 **Heatmap for Hospital Ratings**
- 🏥 **Nearby Hospital Search (with distance filtering)**
- 📈 **Interactive Output Table of Ranked Hospitals**
- 🎨 **User-friendly Web Interface using Flask**

---

## 🧠 How it Works

1. User inputs address, radius, and symptoms via the `/search` form.
2. `model.py` uses a pre-trained classifier (`heart-disease-model.pkl`) to predict a disease and its probability.
3. `Hospital.py` handles:
   - Geocoding the user address
   - Filtering hospitals within the given radius
   - Visualizing results using Plotly and Mapbox
4. Results are displayed in `output.html`, showing:
   - Predicted disease
   - Table of nearby hospitals
   - Embedded interactive map

---

## 🚀 Installation & Setup

### 1. Clone the repository

```bash
git clone https://github.com/RohanDevgon/CareCureMedsML.git
cd CareCureMedsML/CM\ Project
