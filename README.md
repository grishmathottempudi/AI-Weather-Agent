# 🌦️ AI Weather Agent

An AI-powered Weather Assistant built using **Python**, **Gradio**, **Google Gemini API**, and **Open-Meteo API**.

The application accepts a natural language weather query (e.g., *"What's the weather in Hyderabad?"*), extracts the city name using Google's Gemini model, retrieves real-time weather data from Open-Meteo, and generates a friendly weather report.

---

## Features

- 🌍 Understands natural language weather questions
- 🤖 Uses Google Gemini for city extraction
- 📍 Finds city coordinates using Open-Meteo Geocoding API
- ☀️ Retrieves live weather information
- 💬 Generates an easy-to-understand weather summary
- 🖥️ Simple web interface using Gradio

---

## Technologies Used

- Python
- Gradio
- Google Gemini API
- Open-Meteo Geocoding API
- Open-Meteo Weather API
- Requests

---

## Project Structure

```
AI-Weather-Agent/
│
├── app.py
├── requirements.txt
├── README.md
└── screenshots/
    └── demo.png (optional)
```

---

## Installation

### 1. Clone the repository

```bash
git clone https://github.com/yourusername/AI-Weather-Agent.git
cd AI-Weather-Agent
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Add your Gemini API Key

Replace:

```python
client = genai.Client(api_key="YOUR_API_KEY")
```

with your own API key.

---

## Run the Project

```bash
python app.py
```

Gradio will generate a local URL similar to:

```
http://127.0.0.1:7860
```

Open it in your browser.

---

## Example Queries

- What's the weather in Hyderabad?
- Is it raining in Delhi?
- Tell me today's weather in London.
- How is the weather in New York?
- Weather in Tokyo

---

## APIs Used

### Google Gemini API

Used for extracting the city name from the user's natural language query and generating a friendly weather explanation.

### Open-Meteo Geocoding API

Converts a city name into latitude and longitude.

### Open-Meteo Weather API

Provides live weather information including:

- Temperature
- Humidity
- Wind Speed
- Weather Code

---

## Sample Workflow

```
User Query
      │
      ▼
Gemini extracts city
      │
      ▼
Open-Meteo Geocoding API
      │
      ▼
Latitude & Longitude
      │
      ▼
Open-Meteo Weather API
      │
      ▼
Current Weather Data
      │
      ▼
Gemini generates friendly weather report
      │
      ▼
Displayed in Gradio Interface
```

---

## Future Improvements

- 7-day weather forecast
- Weather icons
- Voice input
- GPS-based location detection
- Multiple language support
- Weather maps
- Air Quality Index (AQI)
- Sunrise and sunset timings

---

## Author

**Grishma Thottempudi**

B.Tech - Data Science

---

## License

This project is developed for educational purposes.
