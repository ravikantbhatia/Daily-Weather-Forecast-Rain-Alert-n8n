# 🌦️ Daily Weather Forecast & Rain Alert Automation with n8n

An automated weather monitoring workflow built with **n8n** that retrieves a 5-day weather forecast, processes the forecast data, checks whether rain is expected, and sends a customized email notification every morning.

## 🚀 Project Overview

This workflow automates the process of checking the daily weather forecast and notifying the user by email.

Every morning at **7:00 AM**, the workflow:

1. Triggers automatically.
2. Retrieves a **5-day weather forecast** using the OpenWeatherMap API.
3. Processes the forecast data using an **n8n Code node**.
4. Determines whether rain is expected.
5. Uses conditional logic to choose the appropriate notification.
6. Sends a customized Gmail notification.

## 🔄 Workflow Architecture

```text
Daily 7 AM Trigger
       ↓
OpenWeatherMap API
   (5-Day Forecast)
       ↓
Process Today's Forecast
      (Code Node)
       ↓
   Rain Expected?
     /        \
   YES        NO
    ↓          ↓
Rain Alert   Weather Update
  Gmail         Gmail
🛠️ Technologies Used
n8n – Workflow automation
OpenWeatherMap API – Weather forecast data
JavaScript – Forecast data processing inside the n8n Code node
Gmail – Email notifications
GitHub – Project documentation and version control
✨ Key Features
⏰ Automated Daily Trigger

The workflow runs automatically every morning at 7:00 AM, eliminating the need for manual weather checks.

🌤️ 5-Day Weather Forecast

The workflow retrieves forecast information from the OpenWeatherMap API.

💻 Data Processing

An n8n Code node processes the API response and extracts useful information such as:

City
Weather condition
Temperature
Feels-like temperature
Minimum temperature
Maximum temperature
Humidity
Atmospheric pressure
Wind speed
Cloudiness
🌧️ Rain Detection

The workflow analyzes the forecast and determines whether rain is expected during the day.

📧 Conditional Email Notifications

Depending on the forecast:

If rain is expected → a Rain Alert email is sent.
If rain is not expected → a Weather Update email is sent.
📸 Workflow Screenshots
Complete Workflow

Processed Weather Data

Email Notification

📊 Example Output

The workflow processes the weather API response into structured information such as:

City: Lakhampur
Country: IN
Condition: Broken Clouds
Temperature: 28.53 °C
Feels Like: 30.13 °C
Minimum Temperature: 26.62 °C
Maximum Temperature: 28.53 °C
Humidity: 59%
Pressure: 1008 hPa
Wind Speed: 1.73 m/s
Cloudiness: 65%
Rain Expected: No
🎯 Real-World Use Case

This workflow can be adapted for many automation scenarios, including:

Daily weather notifications
Rain alerts
Travel planning
Outdoor activity alerts
Agricultural weather monitoring
Weather-based business notifications
🔐 Credentials & Security

API keys and Gmail credentials are not included in this repository.

When configuring the workflow, create your own credentials for:

OpenWeatherMap
Gmail

Never commit API keys, passwords, or other sensitive credentials to GitHub.

📁 Project Contents
Daily-Weather-Forecast-Rain-Alert-n8n/
│
├── Daily Weather Forecast & Rain Alert Automation.json
├── Full workflow.png
├── Processed weather data.png
├── Email received.png
└── README.md
👨‍💻 Author

Ravi Kant Bhatia

This project was created as part of my portfolio to demonstrate practical skills in workflow automation, API integration, data processing, and email automation using n8n.

⭐ Project Highlights

Automation: Daily scheduled execution
API Integration: OpenWeatherMap
Data Processing: JavaScript Code Node
Conditional Logic: Rain detection
Notifications: Gmail
Platform: n8n

If you found this project useful, feel free to explore the workflow and adapt it for your own automation requirements.
