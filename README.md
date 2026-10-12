# AI Trip Planner🌍

An AI-powered application that helps plan trips with itineraries, place recommendations, weather information, currency conversion, and expense estimates.

## Features

- Creates day-by-day travel itineraries based on your request
- Recommends attractions, restaurants, activities, and transportation options
- Suggests hotels and approximate nightly prices
- Estimates hotel costs, total trip expenses, and daily budgets
- Retrieves current weather and a short forecast for a destination
- Converts amounts between currencies
- Uses Tavily as a fallback if Google Places search fails
- Provides a Streamlit chat interface
- Uses FastAPI to process requests and return travel plans

Search results, weather, exchange rates, and prices depend on external services. Check important details before booking.

## Technologies

- Python
- Streamlit
- FastAPI and Uvicorn
- LangChain and LangGraph
- Groq
- Google Places, Tavily, OpenWeatherMap, and ExchangeRate-API

## Requirements

- Python 3.11 recommended
- Groq and Google Places API keys
- Optional keys for Tavily, OpenWeatherMap, and ExchangeRate-API

Groq powers the AI assistant. Google Places provides place searches. Tavily is the search fallback. OpenWeatherMap and ExchangeRate-API provide weather and currency features. Add keys for the services you plan to use. Google Places may require billing to be enabled in Google Cloud.

Open the local URL printed by Streamlit, usually `http://localhost:8501`. Keep both terminal windows running while you use the app.

## Example Prompts

```text
Plan a 3-day trip to Goa for two people with a moderate budget.
```

```text
Plan a 5-day trip to Jaipur. Include attractions, restaurants, local transport, weather, and an estimated daily budget.
```

```text
Convert 500 US dollars to Indian rupees.
```

## Screenshots

<img width="1920" height="1200" alt="Screenshot 2026-10-12 184322" src="https://github.com/user-attachments/assets/193e1f5e-19b4-4600-b213-d5d4ffed97b4" />

```

## Project Structure

```text
AI_Trip_Planner-main/
├── agent/             # LangGraph agent workflow
├── config/            # Model configuration
├── prompt_library/    # Travel assistant prompt
├── tools/             # Place, weather, currency, and calculation tools
├── utils/             # API clients and helper functions
├── main.py            # FastAPI backend
├── streamlit_app.py   # Streamlit interface
├── requirements.txt   # Python dependencies
└── .env.example       # Blank API key template
```

## Disclaimer

This app provides AI-generated suggestions and estimates. Confirm current prices, opening hours, weather, transport availability, and travel requirements with the appropriate providers before making plans.
