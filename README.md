# Algorithmic Trading
This project is for Big Data Management (CS226) at UCR with professor Ahmed Eldawy.

In this project, we tested three algorithmic trading strategies on a 10GB stock market data set. The data used for this project is obtained from Kaggle and can be found here: https://www.kaggle.com/paultimothymooney/stock-market-data?select=stock_market_data. The three strategies used are:
- Equal Weight S&P 500 Index Fund
- Quantitative Momentum Investing Strategy
- Quantitative Value Investing Strategy

Prerequisites:
1. Download dataset from https://www.kaggle.com/paultimothymooney/stock-market-data?select=stock_market_data and place the unzipped folder labeled as "stock_market_data" into the same directory as this project. (Note you may need to remain the folder)
2. Check to ensure you have at least [Python 3.8.0](https://www.python.org/doc/versions/) installed on your local system
3. You will also need the following Python libraries to run the notebooks in this project:
    - [Numpy](https://numpy.org/install/)
    - [Pandas](https://pandas.pydata.org/docs/getting_started/install.html)
    - [Requests](https://docs.python-requests.org/en/latest/user/install/)
    - [Apache-Spark](https://spark.apache.org/downloads.html)

Instructions to Run:
1. For each .ipynb python notebook file (equal_weight_S&P_500_list.ipynb, momentum.ipynb, value.ipynb) run each cell within the file starting with the first cell to the last cell
2. Starting portfolio value can be modified for testing purposes by editing the "portfolio_size" variable

