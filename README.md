# 🏛️ Banking Stock Predictor Bot

> AI-powered Telegram bot for institutional-grade stock analysis of the US Banking Sector

Built as part of the **AI in Finance** course — focuses on practical, production-oriented development rather than theory.

---

## 📌 Overview

This bot provides real-time stock predictions and analysis for **JPM, BAC, and WFC** — the three largest US banks. It combines live market data, technical indicators, and Gemini AI reasoning to generate structured investment insights directly in Telegram.

---

## ✨ Features

- 📈 **Multi-Horizon Forecasting** — predictions for Tomorrow, Next Week, and Next Month
- 🤖 **Gemini 2.5 Flash** as the reasoning core — analyzes volatility, macro-factors, and NIM dynamics
- 📊 **Dynamic Charts** — auto-generated technical charts with trend segments (Green/Red/Orange zones)
- 📰 **News Integration** — fetches and processes live news feed for sentiment context
- 🎯 **Confidence Scoring** — internal validation estimates prediction confidence (e.g. 85%)
- ⚡ **Async Architecture** — handles multiple user requests concurrently via `python-telegram-bot`
- 🏦 **Hedge Fund Persona** — specialist analysis framing focused on Fed policy and market pivots

---

## 🛠️ Tech Stack

| Layer | Tool |
|---|---|
| AI Engine | Google Gemini 2.5 Flash |
| Market Data | yfinance (OHLCV real-time) |
| Bot Interface | Telegram Bot API |
| Language | Python (asyncio) |
| Visualization | Matplotlib |
| NLP | Sentiment Analysis on news feed |

---

## 🏗️ Architecture

    User (Telegram)
         │
         ▼
    Bot Handler (asyncio)
         │
         ├── yfinance → OHLCV Data + Technical Indicators
         ├── News Feed → Sentiment Analysis
         │
         ▼
    Gemini 2.5 Flash (AI Reasoning)
         │
         ▼
    Structured Report + Chart PNG → Telegram


⚠️ Disclaimer
Developed for educational purposes as part of the AI in Finance course at Astana IT University. All predictions are AI-generated and do not constitute financial advice.
