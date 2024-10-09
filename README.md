Overview
This project implements a Monte Carlo simulation to estimate the fair value of financial options (call and put) using historical stock price data. The simulation generates multiple potential stock price paths to calculate the expected payoff of options under varying market conditions.




Features
Simulates stock price movements using random sampling.
Estimates fair value of options based on simulated price paths.
Utilizes real historical stock data from Yahoo Finance.
Technologies Used
Programming Language: Python






Libraries
NumPy for numerical computations
Pandas for data manipulation
Matplotlib for data visualization
yfinance for fetching historical stock data
Installation
To set up the project, clone the repository and install the required packages:


Example
Here’s a quick example of how to set up and run the simulation:

python
Copy code
from monte_carlo import calculate_option_price

params = {
    'symbol': 'AAPL',
    'strike_price': 150,
    'risk_free_rate': 0.05,
    'time_to_expiry': 1,
    'iterations': 10000,
    'option_type': 'call'
}

price = calculate_option_price(params)
print(f"Estimated option price: ${price:.2f}")


Contributing
Contributions are welcome! Please open an issue or submit a pull request for any suggestions or improvements.

License
This project is licensed under the MIT License - see the LICENSE file for details.
