# Portfolio-Managment

# Portfolio Optimization Using Python

## Introduction

This project demonstrates the use of portfolio optimization to balance risk and return in investment portfolios. Portfolio optimization is a fundamental concept in finance, helping investors manage risk and maximize returns on their investments. This tutorial focuses on using Python to perform portfolio optimization, covering data collection, data preparation, metric calculation, Monte Carlo simulations, and optimization algorithms.

## Sections Overview

### 1. Data Collection

The first step involves collecting the necessary data for analysis. In this project, we focus on obtaining closing price data for a small portfolio of stocks listed on the NASDAQ. The symbols used in this example are:

- ITUB4.SA (Itaú Unibanco Holding S.A.)
- BBDC4.SA (Banco Bradesco S.A.)
- ABEV3.SA (Ambev S.A.)
- PETR3.SA (Petróleo Brasileiro S.A. - Petrobras)
- VALE3.SA (Vale S.A.)

The data is fetched and stored for further processing.

### 2. Data Preparation

Once the data is collected, it needs to be prepared for analysis. The data is reorganized to create a table where each column represents the closing prices of a particular stock. This format facilitates the calculation of daily returns for each stock.

### 3. Metrics Calculation

To optimize a portfolio, it is essential to calculate several key metrics:
- **Expected Returns:** The average return expected from the portfolio.
- **Expected Volatility:** The standard deviation of the portfolio's returns, representing risk.
- **Sharpe Ratio:** A measure of risk-adjusted return, calculated as the expected return divided by the expected volatility.

### 4. Monte Carlo Simulation

Monte Carlo simulations are used to model the probability of different outcomes in a process with random variables. In this project, we run thousands of simulations to generate random portfolio allocations and calculate the associated returns, volatility, and Sharpe ratios. The results are stored and analyzed to find the optimal portfolio.

### 5. Optimization Algorithm

While Monte Carlo simulations provide a broad overview of potential outcomes, they are not the most efficient method for finding optimal values. Instead, we use mathematical optimization techniques. Specifically, the scipy.optimize module is used to minimize the negative Sharpe ratio and the portfolio volatility. Constraints and bounds are defined to ensure that the sum of the portfolio weights equals 100%.

## Conclusion

This project demonstrates how to use Python for portfolio optimization, leveraging data collection, preparation, Monte Carlo simulations, and optimization algorithms. By following this methodology, investors can balance risk and return to achieve their financial objectives. The theoretical concepts and methods covered in this project provide a solid foundation for implementing portfolio optimization in real-world scenarios.