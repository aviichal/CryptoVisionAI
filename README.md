# CryptoVisionAI
CryptoVisionAI is a cryptocurrency trading assistant that provides both manual and automated trading functionalities. It enables users to trade popular cryptocurrencies, predict future prices using LSTM models, manage their portfolio, and detect suspicious trading activities through fraud detection algorithms. This application is designed to help users optimize their cryptocurrency investments with AI-powered tools and features.

**Features**

**User Registration and Authentication:** Allows users to securely register and log in using hashed passwords.

**Portfolio Management:** Users can add cryptocurrencies to their portfolio, view current holdings, and monitor their investments.

**Manual Trading:** Users can manually buy cryptocurrencies by specifying the price and quantity, and the system deducts the cost from their virtual bank balance.

**Auto-Buy (Crypto Assistant):** Based on LSTM model price predictions, the system automatically buys cryptocurrency if the expected profit meets the user's target.

**LSTM-based Price Prediction:** Utilizes an LSTM neural network to predict future cryptocurrency prices based on historical data fetched from CoinGecko API.

**Fraud Detection:** Implements an Isolation Forest algorithm to detect potentially fraudulent trades based on trade history and anomalies.

**Tech Stack**

Python: The main programming language for the project.

TensorFlow/Keras: Used for building and training the LSTM model for price prediction.

sklearn: Provides the Isolation Forest for fraud detection and data preprocessing tools.

Pandas and NumPy: Used for handling cryptocurrency data and performing data manipulation tasks.

CoinGecko API: Fetches historical cryptocurrency data for price prediction.

Matplotlib: For plotting predicted price trends.

Hashlib: Ensures secure password hashing during user registration.

**How it Works**

**1. User Registration and Login**
Users can register an account by providing their email, full name, password, and an initial bank balance. Passwords are hashed using SHA-256 for security. After registering, users can log in to access the main dashboard.

**2. Manual Cryptocurrency Trading**
Once logged in, users can choose to manually trade cryptocurrencies from the list of supported coins (e.g., Bitcoin, Ethereum, Litecoin, etc.). They specify the quantity and price at which they want to buy, and the system updates their portfolio accordingly while deducting the amount from their virtual bank balance.

**3. Auto-Buy Using AI Predictions**
The auto-buy feature uses an LSTM model to predict the future price of selected cryptocurrencies based on the last 365 days of price history. If the predicted profit exceeds the user-defined profit target, the system automatically buys the cryptocurrency and updates the portfolio.

**4. Portfolio Management**
Users can view all their current holdings, including the name of the cryptocurrency, the quantity held, and the purchase price for each asset.

**5. Fraud Detection**
The system utilizes an Isolation Forest algorithm to identify potentially fraudulent trades. It detects outliers in trade activity by analyzing the quantity and price of trades, alerting users if any suspicious activity is detected.

**Supported Cryptocurrencies**

Bitcoin

Ethereum

Litecoin

Ripple

Cardano

**Future Enhancements**

Buy and Sell Functionality: Expand the trading capabilities to include selling assets.

Real-time Price Monitoring: Add real-time price tracking for cryptocurrencies.

Enhanced Fraud Detection: Improve fraud detection using more advanced anomaly detection algorithms.

Web Interface: Build a web-based interface for easier interaction.
