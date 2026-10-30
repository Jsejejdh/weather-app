# weather-app
# Weather Forecast App

A Python desktop application that retrieves and displays **real-time weather data** with **automatic user location detection** and a clean, user-friendly interface.

Built as part of my internship at **Pinnacle Labs**.

---

## Features

**Automatic location detection** using IP geolocation
**City search** to check the weather anywhere in the world
**Real-time weather data**: temperature, feels-like, humidity, wind speed
**Today's forecast**: high/low temperature and chance of rain
**Simple GUI** built with Tkinter
**Responsive UI**: network calls run in background threads so the app never freezes

## Tech Stack

| Purpose | Technology |
|---|---|
| Language | Python 3 |
| GUI | Tkinter |
| HTTP requests | `requests` |
| Weather data | [Open-Meteo API](https://open-meteo.com/) (free, no key needed) |
| Location detection | [ip-api.com](https://ip-api.com/) (free, no key needed) |
| City geocoding | Open-Meteo Geocoding API |

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/Jsejejdh/weather-forecast-app.git
   cd weather-forecast-app
   ```

2. Install the dependency:
   ```bash
   pip install requests
   ```

3. Run the app:
   ```bash
   python weather_app.py
   ```

> Tkinter ships with most Python installations. On some Linux distros, install it with `sudo apt install python3-tk`.

## How It Works

1. On launch, the app detects your approximate location from your public IP.
2. It sends the coordinates to the Open-Meteo forecast API.
3. The response is parsed and shown in a weather card with an icon, temperature, condition and extra details.
4. You can also type any city name; the app geocodes it and fetches the weather for that place.

## Project Structure

```
weather-forecast-app/
├── weather_app.py   # Main application
└── README.md
```

## Possible Improvements

- 5-day / hourly forecast view
- °C / °F unit toggle
- Save favourite cities
- Weather-based background themes

## Author

**Shreya Pandey**
B.Tech CSE | Sarala Birla University
GitHub: [@Jsejejdh](https://github.com/Jsejejdh)
LinkedIn: [Shreya Pandey](https://www.linkedin.com/in/shreya-pandey-497b99294/)
