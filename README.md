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
Build and deploy a production AccuWeather-style weather dashboard for
Bengaluru, India. Create ./weather-dashboard/index.html as a complete
single-file HTML app that fetches live weather from Open-Meteo API, shows
current temperature, hourly forecast, 7-day forecast, and weather stats.
Build a Docker image using nginx:alpine, run it on port 8080, and confirm
it is live at http://localhost:8080
```
