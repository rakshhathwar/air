🌍 Air Quality Tracker

A modern Streamlit web app that monitors and predicts Air Quality Index (AQI) globally in real time using data from the OpenWeatherMap API.

It calculates live pollutant levels (PM2.5, PM10, O₃, CO, NO₂, SO₂), classifies AQI bands, and predicts the next 4-hour air quality trend using an optimized XGBoost regression model — all displayed with a beautiful, modern UI featuring gradient cards and health recommendations.

------------------------------------------------------------

🚀 Features
- Fetches real-time air pollution and weather data from OpenWeather API
- Calculates AQI and provides human-readable labels (Good, Moderate, Unhealthy, etc.)
- Predicts the next 4-hour pollutant trend using XGBoost
- Dynamic Plotly visualizations
- Beautiful gradient UI with color-coded AQI cards
- Health recommendations based on AQI category
- Supports any global city or custom latitude/longitude
- Downloadable CSV data snapshots
- Cached API calls for faster response  

------------------------------------------------------------

🧩 Tech Stack
- Frontend/UI: Streamlit + Plotly  
- Backend: Python  
- ML Model: XGBoost + Scikit-Learn  
- Data Source: OpenWeatherMap Air Pollution API  

------------------------------------------------------------

🛠️ Setup Instructions

1️⃣ Clone this repo
git clone https://github.com/rakshhathwar/Air-quality
cd Air-quality

2️⃣ Create virtual environment
python -m venv venv
venv\Scripts\activate # on Windows

or
source venv/bin/activate # on macOS/Linux

3️⃣ Install dependencies
pip install -r requirements.txt

4️⃣ Add your OpenWeather API key
Create `.streamlit/secrets.toml` and add:
OPENWEATHER_API_KEY = "your_api_key_here"

5️⃣ Run the app
streamlit run app.py

Then open http://localhost:8501 in your browser.

------------------------------------------------------------

🌐 Deployment
This app can be deployed on Streamlit Cloud easily:
1. Connect your GitHub repo
2. Set main file path as `app.py`
3. Add the same API key in App Secrets:
OPENWEATHER_API_KEY="your_api_key_here"
4. Click Deploy

------------------------------------------------------------

📁 Project Structure
```
Air-quality/
├── .streamlit/
│   └── secrets.toml          # API key configuration (not in git)
├── app.py                    # Main Streamlit application
├── requirements.txt          # Python dependencies
├── .gitignore               # Git ignore file
└── README.md               # Project documentation
```

------------------------------------------------------------

� API Key Setup
Get your free API key from https://openweathermap.org/api and add it to `.streamlit/secrets.toml`. Note that new API keys may take up to 2 hours to activate.  
