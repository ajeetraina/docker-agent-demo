## Weather Dashboard Demo

## Clone the repository

```
git clone https://github.com/ajeetraina/weather-dashboard-docker-agent/
```

## Using Docker agent

```
cd weather-dashboard-docker-agent/
docker agent run docker-agent.yaml
```


## Prompt

```
Build a production-grade AccuWeather-style weather dashboard for Bengaluru, India as a single self-contained HTML file.

Requirements:
- Real-time weather display for Bengaluru using the Open-Meteo API (free, no API key needed): https://api.open-meteo.com/v1/forecast?latitude=12.9716&longitude=77.5946&current=temperature_2m,relative_humidity_2m,apparent_temperature,weather_code,wind_speed_10m,precipitation&hourly=temperature_2m,weather_code&daily=weather_code,temperature_2m_max,temperature_2m_min,precipitation_sum&timezone=Asia/Kolkata

UI sections to build:
1. Hero section - Current temperature, feels like, weather condition, city name
2. Hourly forecast - Next 12 hours with icons and temperature
3. 7-day forecast - Daily high/low with weather icons
4. Weather stats grid - Humidity, Wind Speed, Precipitation, UV Index
5. Animated weather background that changes based on condition (sunny, cloudy, rainy)

Design:
- Dark navy/midnight blue theme like AccuWeather
- Smooth CSS animations and transitions
- Weather condition icons using Unicode emoji or SVG
- Responsive layout for desktop and mobile
- Glassmorphism cards with subtle blur effects
- Show last updated timestamp

Save the complete working HTML to ./weather-dashboard/index.html and then serve it using: docker run -d -p 8080:80 -v $(pwd)/weather-dashboard:/usr/share/nginx/html nginx:alpine

Confirm the dashboard is accessible at http://localhost:8080
```
