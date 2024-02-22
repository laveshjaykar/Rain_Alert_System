# Weather Alert System

This Python script is designed to check the weather forecast for the next 12 hours and send an alert message if there is any indication of rain. It utilizes the OpenWeatherMap API for weather data and Twilio's API for sending SMS alerts.

How It Works

Environment Variables: The script uses environment variables to securely store sensitive information such as Twilio account SID, auth token, and OpenWeatherMap API key.
OpenWeatherMap API: It sends a request to the OpenWeatherMap API with specified parameters including latitude, longitude, and excluded data parts to fetch weather data.
Weather Analysis: The script processes the hourly forecast for the next 12 hours, checking for weather conditions with IDs less than 700, which indicate rain.
Twilio SMS Alert: If rain is forecasted within the next 12 hours, the script uses Twilio's client to send an SMS alert notifying the recipient to carry an umbrella.
