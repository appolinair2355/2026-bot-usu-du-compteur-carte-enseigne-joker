# Telegram Baccarat Prediction Bot

## Overview
A Telegram bot for Baccarat game predictions. The bot monitors a source channel for game results and sends predictions to a prediction channel based on pattern analysis.

## Project Structure
- `main.py` - Main bot application with Telegram client and prediction logic
- `config.py` - Configuration file loading environment variables
- `requirements.txt` - Python dependencies

## Technologies
- Python 3.11
- Telethon (Telegram client library)
- aiohttp (Web server for health checks)

## Configuration
The bot requires the following environment variables (stored as secrets):
- `API_ID` - Telegram API ID
- `API_HASH` - Telegram API Hash  
- `BOT_TOKEN` - Telegram Bot Token
- `ADMIN_ID` - Telegram Admin User ID (optional)
- `SOURCE_CHANNEL_ID` - Source channel to monitor
- `PREDICTION_CHANNEL_ID` - Channel to send predictions to
- `TELEGRAM_SESSION` - Session string (optional)

## How It Works
1. Monitors the source channel for finalized game results
2. Analyzes card suits in game results
3. Uses pattern matching to predict future game outcomes
4. Sends predictions to the prediction channel
5. Tracks and updates prediction results (win/loss)

## Running the Application
The application runs on port 5000 with a simple web interface for health checks.

## Recent Changes
- January 15, 2026: Initial setup for Replit environment
