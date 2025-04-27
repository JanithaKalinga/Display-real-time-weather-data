# Weather Data Dashboard
Project Overview
This project is a real-time Weather Monitoring Dashboard of a user provided location built using Node-RED and the OpenWeatherMap API. It provides live updates of critical weather parameters such as temperature, humidity, pressure, wind speed, and wind direction, all beautifully visualized through interactive gauges, charts, and text displays. The dashboard also allows users to set custom warning limits for each parameter and receive automatic notifications when limits are exceeded.
Features
🌡️ Temperature Monitoring:
Displayed via a gauge (0–50°C) and a real-time line chart.

💧 Humidity Monitoring:
Displayed via a wave gauge (0–100%) and a humidity chart.

🌬️ Wind Speed and Direction:

Wind speed shown on a gauge (0–25 km/h) and a real-time chart.

Wind direction shown graphically with a dynamic rotating compass.

🌞 Sunrise and Sunset Times:
Displayed in real-time using the local timezone.

🌐 Flexible Location Input:

Select weather based on City/Country or Latitude/Longitude.

Easily switch input mode using a dropdown menu.

⏰ Customizable Refresh Interval:
Set how frequently data updates (in seconds) from the UI.

📈 Chart Enable/Disable Toggle:
Users can enable or disable historical weather charts with a simple switch.

⚠️ Custom Warning System:

Set personalized limits for Temperature, Humidity, Pressure, and Wind Speed.

Get instant visual and text notifications if any limit is exceeded.

🔊 Voice Output:
Weather description is audibly read out using Microsoft David (US English voice).

Dashboard Sections
Weather Tab:

Gauges for Temperature, Humidity, Pressure, Wind Speed.

Wind Direction Compass.

Sunrise/Sunset Times.

Weather Description.

Settings Tab:

Update the data refresh interval.

Switch between city/country or coordinates input.

Enable/Disable charts.

Charts Tab:

Real-time line charts for Temperature, Humidity, and Wind Speed.

Chart status display (Enabled/Disabled).

How it Works
Weather Data Fetching:
Weather data is fetched from OpenWeatherMap at the user-defined intervals.

Data Processing:
Extracted parameters are processed through function nodes for unit conversions and formatting (e.g., pressure in atm, wind speed in km/h).

Visualization:
Data is displayed using Node-RED Dashboard nodes such as ui_gauge, ui_chart, ui_text, and ui_template.

Warning System:
User-set warning thresholds are compared against real-time weather data to trigger alerts.

