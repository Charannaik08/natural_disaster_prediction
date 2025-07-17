
---

```markdown
# 🌍 Natural Disaster Prediction Web App

A web-based application that predicts the type of natural disaster (e.g., Earthquake, Flood, Tsunami, etc.) based on real-world parameters like location, magnitude, and year. This system uses a trained Machine Learning model, a Flask backend, and a MySQL database with login/registration support.

## 🚀 Features

- 🔐 User Registration and Login with password hashing
- 🌍 Predicts disaster type based on:
  - Year
  - Disaster Magnitude Scale & Value
  - Country
  - Latitude and Longitude
- 🧠 Trained Random Forest Model for prediction
- 📍 Map-based disaster location visualization using OpenStreetMap
- 📌 Reverse geocoding to identify location from coordinates
- 📂 Data stored and managed using MySQL
- 🎨 Stylish and responsive UI

---

## 🛠️ Tech Stack

| Layer         | Tools/Frameworks                       |
|---------------|----------------------------------------|
| Frontend      | HTML, CSS, Jinja2, Leaflet.js          |
| Backend       | Python, Flask                          |
| Machine Learning | Scikit-learn, imbalanced-learn, NumPy |
| Database      | MySQL                                  |
| Mapping       | OpenStreetMap & Leaflet.js             |

---

## 📂 Project Structure

```

project/
│
├── templates/
│   ├── index.html          # Prediction input form
│   ├── login.html          # Login page
│   ├── register.html       # Registration form
│   └── result.html         # Displays prediction + map
│
├── static/
│   └── css/
│       └── styles.css      # Stylesheet
│
├── random\_forest\_model.joblib  # Saved ML model
├── scaler.joblib               # Saved scaler
├── app.py                      # Main Flask application
├── requirements.txt
└── README.md

````

---

## ⚙️ Installation & Setup

1. **Clone the Repository**
```bash
git clone [https://github.com/your-username/natural-disaster-prediction.git
cd natural-disaster-prediction](https://github.com/Charannaik08/natural_disaster_prediction/edit/main/README.md)
````

2. **Create a virtual environment**

```bash
python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate
```

3. **Install Requirements**

```bash
pip install -r requirements.txt
```

4. **Configure MySQL Database**

```sql
CREATE DATABASE disaster_app;
USE disaster_app;

CREATE TABLE users (
    id INT AUTO_INCREMENT PRIMARY KEY,
    username VARCHAR(255) NOT NULL,
    email VARCHAR(255) NOT NULL,
    password VARCHAR(255) NOT NULL
);
```

5. **Run the App**

```bash
python app.py
```

Visit: `http://127.0.0.1:5000`

---

## 📊 Dataset & Model

* Dataset: Preprocessed disaster data (e.g., year, location, magnitude, type).
* Model: Random Forest Classifier trained on disaster features.
* Oversampling: Done using `RandomOverSampler` from `imblearn`.

---

## 📌 Future Enhancements

* Add admin dashboard for tracking all predictions
* Store prediction history per user
* Add disaster response tips per disaster type
* Use real-time data from APIs (e.g., weather or seismic)
* Improve model accuracy using deep learning techniques

---

## 🙏 Acknowledgements

* [OpenStreetMap](https://www.openstreetmap.org/) for free map data
* [Scikit-learn](https://scikit-learn.org/) for ML
* [Flask](https://flask.palletsprojects.com/) for backend
* [Leaflet.js](https://leafletjs.com/) for map rendering

---

## 🧑‍💻 Author

**Charan Naik**
MCA Student, Presidency College, Bengaluru
🌐 [LinkedIn](https://www.linkedin.com/in/your-profile/)
📧 [charan@example.com](mailto:charan@example.com)

---


