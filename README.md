# Project Overview

In this project, I developed a Personal Finance and Retirement Planning Tool for a credit union, with the goal of helping its members enhance their financial health. The tool consists of two main parts:

1. Personal Finance Planner: This section allows users to assess their monthly personal finances, including savings in cryptocurrencies, stocks, and bonds. Users can visualize their savings composition and check if they have enough money for an emergency fund.

2. Retirement Planning Tool: In this section, I use historical data and Monte Carlo simulations to project the performance of a retirement portfolio composed of stocks and bonds over 30 years. I also provide analysis and insights into retirement planning.

# Tools and APIs Used

To build this tool, I utilized the following tools and APIs:

- **Python**: I used Python as the primary programming language for data collection, analysis, and visualization.

- **Jupyter Notebook**: The project was organized into a Jupyter Notebook to facilitate step-by-step development.

- **Alpaca Markets API**: I used the Alpaca API to retrieve historical closing prices for stocks (SPY) and bonds (AGG).

- **Alternative Free Crypto API**: This API was used to fetch the current prices of Bitcoin (BTC) and Ethereum (ETH).

- **MCForecastTools Toolkit**: This toolkit alloId us to perform Monte Carlo simulations for retirement planning.

# Part 1 - Personal Finance Planner

In this section, I focused on assessing the financial health of credit union members and helping them plan for emergencies.

**Steps Taken:**

1. **Collect Crypto Prices**: I obtained the current prices of Bitcoin and Ethereum using the Alternative Free Crypto API.

2. **Collect Investments Data Using Alpaca**: I retrieved the current closing prices for stocks (SPY) and bonds (AGG) using the Alpaca API.

3. **Savings Health Analysis**: I assessed the total value of savings in cryptocurrencies and stocks/bonds. I then used this data to plot a pie chart showing the composition of personal savings. I also checked if the savings Ire enough for an emergency fund.

# Part 2 - Retirement Planning

In this section, I focused on helping credit union members plan for their retirement by simulating portfolio performance over 30 years.

**Steps Taken:**

1. **Monte Carlo Simulation**: I fetched historical closing prices for a 40/60 portfolio (60% stocks - SPY, and 40% bonds - AGG) using the Alpaca API. I configured and executed a Monte Carlo simulation with 500 runs and 30 years. I visualized the results, including probability distributions and confidence intervals.

2. **Retirement Analysis**: I computed summary statistics from the Monte Carlo simulation results. I calculated the expected portfolio return at the 95% lower and upper confidence intervals for an initial investment of $20,000. Additionally, I explored how a 50% increase in the initial investment would affect expected returns.

# Part 3 - Early Retirement

To address the early retirement option, I make adjustments to the portfolio, such as increasing the stock-to-bond ratio (taking an initial investment of $30,000 & the ratio of 80/20 portfolio - for 5 years) or increasing the initial investment (taking an initial investment of $60,000 & the ratio of 60/40 portfolio - for 10 years). After these adjustments, I rerun the retirement analysis to determine what it would take to retire in 5 or 10 years instead of the original 30-year plan.

