# 🚴 Rider Assistant System

A beginner-friendly data science project that helps riders choose the safest and most efficient route based on real-time **weather**, **traffic**, and **accident risk**. Ideal for solo travelers, bikers, and city riders looking for safe and efficient routes — from remote terrains like Leh–Ladakh to busy urban roads.

---

## 📌 Features

- 📍 Takes start and destination location from the user
- 🌧️ Fetches weather conditions
- 🚦 Analyzes traffic congestion
- 🚑 Considers accident history on routes
- 🧠 Calculates a risk score for each route
- 🗺️ Recommends the best (safest + fastest) route

---

## 🧠 Technologies Used

| Category         | Tools / Libraries                    |
|------------------|--------------------------------------|
| Programming      | Python 3.x                           |
| Data Analysis    | Pandas, NumPy                        |
| Machine Learning | scikit-learn, XGBoost (optional)     |
| Web APIs         | OpenWeatherMap API, Google Maps API  |
| Visualization    | Matplotlib, Folium                   |
| Web App (Optional)| Streamlit                           |
| Version Control  | Git, GitHub                          |


---


## 📁 Project Structure

| Folder / File         | Description                                      |
|------------------------|--------------------------------------------------|
| `data/`               | Datasets (CSV, JSON, cleaned/raw data)           |
| `notebooks/`          | Jupyter notebooks for EDA and model building     |
| `src/`                | Source code: functions, model logic, utils       |
| `app/`                | Streamlit app (optional UI to interact with model)|
| `images/`             | Flowcharts, screenshots, visual outputs          |
| `README.md`           | Project overview and instructions                |
| `requirements.txt`    | Python dependencies                              |
| `.gitignore`          | Files/folders to exclude from Git versioning     |

## 🚀 How to Run the Project

### 1. Clone the repository
```bash
git clone https://github.com/your-username/rider-assistant-system.git
cd rider-assistant-system
```

### 2. Install Required Libraries
#### Make sure you have Python installed (preferably 3.8 or higher). Then install the required dependencies using:

```bash
pip install -r requirements.txt
```

### 3. Run the Code
Open and explore notebooks located in the notebooks/ directory.
(Optional) If you're using the Streamlit interface, navigate to the app/ folder and run:

```bash
streamlit run app.py
```
### 4. Set Up API Keys (If Using External APIs)
Create a .env file in the root directory and add your API keys:

```bash
WEATHER_API_KEY=your_openweathermap_key
GOOGLE_MAPS_API_KEY=your_google_maps_key
```

## 🧠 How It Works

1. User inputs source and destination.
2. The system fetches real-time weather and traffic data via external APIs.
3. Accident data and risk-prone zones are checked using historical datasets.
4. A risk score is calculated for multiple route options based on:
   - Weather severity
   - Traffic congestion
   - Accident density
5. The route with the **lowest risk score** is recommended to the rider.


## 🔗 APIs and Datasets Used

- 🌦️ [OpenWeatherMap API](https://openweathermap.org/api) – for live weather data  
- 🗺️ [Google Maps Directions API](https://developers.google.com/maps/documentation/directions) – for route planning  
- 🚦 [TomTom Traffic API](https://developer.tomtom.com/) *(or alternative)* – for real-time traffic
- 📊 Accident history dataset – (e.g., from Kaggle or Open Government Data platform)

## 📄 License

This project is licensed under the MIT License.  
Feel free to use, modify, and distribute this project.

