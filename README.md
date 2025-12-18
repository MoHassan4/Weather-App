# 🌦️ Weather App (React + Vite)

A modern and interactive **Weather Application** built with **React + Vite** that allows users to search for real-time weather information for any city worldwide. The app features dynamic backgrounds that change based on weather conditions and day/night status.

---

## 🚀 Features

* 🔍 City search with **autocomplete suggestions**
* 🌡️ Temperature display with **Celsius / Fahrenheit toggle**
* 🌬️ Detailed weather information:

  * Humidity
  * Wind speed & direction
  * Visibility
  * Sunrise & Sunset times
* 🎨 Dynamic background based on weather condition
* ✨ Smooth animations using Tailwind CSS
* ⚠️ Error handling for invalid or empty searches

---

## 🛠️ Tech Stack

* **React** (Hooks: `useState`, `useEffect`)
* **Vite**
* **Tailwind CSS**
* **OpenWeatherMap API**
* **Geocoding API** (for city suggestions)

---

## 📁 Project Structure

```
src/
├── components/
│   ├── Icons.jsx
│   ├── Helper.js
│   └── WeatherBackground.jsx
├── assets/
│   ├── wind.png
│   ├── humidity.png
│   └── ...
├── App.jsx
└── main.jsx
```

---

## 🔑 Environment Variables Setup

Create a `.env` file in the root of the project and add:

```env
VITE_WEATHER_API_KEY=your_openweather_api_key
```

> ⚠️ When using Vite, environment variables **must** start with `VITE_`

---

## ▶️ Running the Project Locally

```bash
# Install dependencies
npm install

# Start development server
npm run dev
```

Then open your browser at:

```
http://localhost:5173
```

---

## 🧠 Application Logic Overview

* When the user types a city name (minimum 3 characters):

  * The **Geocoding API** is called to fetch city suggestions
* When a city is selected or searched:

  * Weather data is fetched from the **OpenWeatherMap API**
* Helper functions are used to format and convert data, such as:

  * `convertTemperature`
  * `getWindDirection`
  * `getVisibilityValue`

---

## 📡 API Example

```http
https://api.openweathermap.org/data/2.5/weather?q=London&appid=API_KEY&units=metric
```

---

## 📡 Live Demo 
```http
https://weather-app-openweather-apis.netlify.app/
```
## 📌 Future Improvements

* 🌍 GPS-based location detection
* 📅 5-day / 7-day weather forecast
* 🌙 Dark / Light mode
* 🌐 Multi-language support
* 📱 Enhanced mobile responsiveness

---

## 👨‍💻 Developer

This project was built for learning and practical application of:

* React Hooks
* API integration
* UI/UX best practices

---

## ⭐ Notes

If you like this project, don’t forget to give it a ⭐️ on GitHub!
Suggestions and improvements are always welcome 🤍

---

**Happy Coding! 🚀**
