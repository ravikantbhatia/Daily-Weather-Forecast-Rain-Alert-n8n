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
      /       \
    YES        NO
     ↓          ↓
Rain Alert   Weather Update
   Email         Email
