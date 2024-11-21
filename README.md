## Black-Scholes Model

The **Black-Scholes Model** is a mathematical model used to price European-style options. This repository contains the implementation of the Black-Scholes pricing formula to calculate the theoretical price of a call or put option, given certain market parameters.

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Contributors](#contributors)
- [License](#license)

## Introduction
The **Black-Scholes Model** is one of the most widely used methods for options pricing. This model provides a closed-form solution for pricing European-style options, taking into account factors such as the stock price, strike price, time to expiration, risk-free interest rate, and the volatility of the underlying asset.

In this project, the Black-Scholes formula has been implemented in Python, enabling users to calculate the theoretical price of call and put options efficiently.

## Features
- **Option Pricing:** Calculates both call and put option prices based on the Black-Scholes formula.
- **Dynamic Parameters:** Users can input their own values for stock price, strike price, time to expiration, volatility, and risk-free interest rate.
- **User-Friendly:** Easy-to-use interface for option pricing and quick results.

## Installation

To run the Black-Scholes model, clone the repository and install the necessary dependencies.

```bash
git clone https://github.com/ByteBabe-69/blacksholes-main.git
cd blacksholes-main
```

You will need to have Python 3.x installed. Install the required dependencies by running:

```bash
pip install -r requirements.txt
```

## Usage

Once you have installed the necessary dependencies, you can run the script to calculate option prices. 

### Example:
```python
from blackscholes import calculate_call_price, calculate_put_price

# Define input parameters
S = 100  # Stock price
K = 95   # Strike price
T = 1    # Time to expiration in years
r = 0.05 # Risk-free interest rate
sigma = 0.2 # Volatility of the stock

# Calculate call and put option prices
call_price = calculate_call_price(S, K, T, r, sigma)
put_price = calculate_put_price(S, K, T, r, sigma)

print(f"Call Option Price: {call_price}")
print(f"Put Option Price: {put_price}")
```

### Output:
```
Call Option Price: 10.4507
Put Option Price: 4.2356
```

You can modify the input parameters (`S`, `K`, `T`, `r`, and `sigma`) to reflect different options and market conditions.

## Contributors
- [Your Name or Username](https://github.com/ByteBabe-69)
