# 30 Days DevOps Challenge - Weather Dashboard
Day 2: Building a Game data notification system using Azure Function App, Blob Storage, EventGrid, Logic App, Outlook, and SportsData.io API

# Game Data Notificaion System - DevOps Day 2 Challenge
![Project Structure](./DevopsChallenge_day02.drawio.png)

## Project Overview
This project automates fetching sports updates from a sports API, processes the data, and sends email notifications to emails using Azure services.

- External API Integration [Link to Sportsdata website](http://sportsdata.io/ "Sportsdata.io API")
- Azure Function App,
- Azure EventGrid
- Azure Logic App
- Version Control (Git)
- Python Development
- Error Handling
- Environment Management

## Features
- The timer trigger in the function app triggers a fetch of sports data from the Sportsdata API
- Processes the data to the suitable format
- Sends the data to the EventGrid which has a topic/subscriber feature
- The Logic App which is subscribed to the EventGrid topic receives the data from the EventGrid and sends an email with Outlook

## Prerequisites
- Python 3.x
- Azure Managed Identity
- OpenWeather API key

## Dependencies
- python-dotenv
- requests
- azure-eventgrid
- azure-functions
- python-dotenv

## Project Structure
```shell
01_weather_dashboard/g
├── function_app.py
├── .gitignore
├── .funcignore
├── .host.json
├── .env
├── requirements.txt
└── README.md
```
