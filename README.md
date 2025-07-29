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

### 2. Install Dependencies

```bash
pip install -r requirements.txt
If requirements.txt is not available, install manually:

bash
Copy
Edit
pip install flask pandas numpy plotly geopy requests joblib
3. Run the Flask App
bash
Copy
Edit
python app.py
Then open your browser and go to:
👉 http://127.0.0.1:5000/

🔍 Example Screenshots
Home Page with Rating Map

Search Form with Symptoms

Disease Prediction Output

Nearby Hospital Heatmap

(Screenshots in /static/screenshots/ if available)

📌 Dataset Info
The project uses:

Training1.csv & Testing1.csv: For disease prediction

Hospital_data.csv: Real US hospital ratings (CMS)

Hospital_General_Information.csv: For enrichment

⚙️ Technologies Used
Frontend: HTML, CSS (Flask + Jinja Templates)

Backend: Python, Flask

ML: scikit-learn (model loaded via joblib)

Maps: Plotly + Mapbox, OpenStreetMap, Geopy

APIs: Positionstack, Nominatim for geocoding

🛠️ Future Improvements
🧬 Expand disease prediction model to broader symptoms

📄 Add PDF export of results

🔒 Add authentication for user history

📦 Deploy on Render/Heroku with live maps

⚠️ Disclaimer
This tool is intended for educational and informational purposes only.
It should not be used as a substitute for professional medical advice or diagnosis.

🙌 Acknowledgments
Inspired by CMS hospital datasets

Map visualizations powered by Plotly + Mapbox

Geocoding via Nominatim & Positionstack API
