ALGO_Trading_Project
Welcome to the ALGO Trading Project, a comprehensive algorithmic trading prototype designed to simulate and execute trading strategies using Python and FastAPI for the backend, with a React-based frontend for visualization. This project leverages financial data from Yahoo Finance and optionally Alpaca API for real-time trading capabilities.
Overview
This repository contains a full-stack application for algorithmic trading, including:

Backend: A FastAPI server with trading logic, backtesting, and live data streaming.
Frontend: A React application with Tailwind CSS for an intuitive trading dashboard.
Database: SQLite for storing trade history.

Prerequisites
Before cloning and running the project, ensure you have the following installed:

Python 3.8+
Node.js 14+
npm (Node Package Manager)

Optional

Alpaca API credentials (for live trading features).

Installation
1. Clone the Repository
git clone https://github.com/ManavChauhan123/ALGO_Trading_Project.git
cd ALGO_Trading_Project

2. Backend Setup

Navigate to the backend directory:cd backend


Create a virtual environment and activate it:python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate


Install Python dependencies:pip install -r requirements.txt


(Optional) Set up Alpaca API credentials:
Create a .env file in the backend directory.
Add your Alpaca API key and secret:ALPACA_API_KEY=your_api_key
ALPACA_SECRET_KEY=your_secret_key





3. Frontend Setup

Navigate to the frontend directory:cd ../frontend


Install Node dependencies:npm install



Running the Project
1. Start the Backend

From the backend directory, run the FastAPI server:uvicorn main:app --reload


The server will be available at http://127.0.0.1:8000.

2. Start the Frontend

From the frontend directory, run the React app:npm start


The app will open in your default browser at http://localhost:3000.

3. Access the Application

Use the frontend to interact with the trading system, including backtesting strategies and viewing live data (if Alpaca is configured).

Features

Backtesting: Test trading strategies (SMA Crossover, RSI, Bollinger Bands) with customizable parameters.
Live Data: Stream real-time stock prices using Alpaca API or simulated data from Yahoo Finance.
Trade History: Store and retrieve trade details in a SQLite database.
Price Prediction: Use LSTM models to predict future stock prices.
WebSocket Support: Real-time updates via WebSocket connections.

Usage

Explore the /backtest API endpoint to run backtests with different strategies.
Use the /ws/live/{symbol} WebSocket to stream live data for a specific stock symbol.
View trade history and performance metrics via the /trades/{symbol} endpoint.

Contributing
Feel free to fork this repository, submit issues, or create pull requests. Contributions to enhance strategies, UI, or performance are welcome!
License
This project is licensed under the MIT License.
Contact
For questions or support, reach out to ManavChauhan123.
