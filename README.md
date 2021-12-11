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

A requirements.txt file has been included so that running <pip install -r requirements.txt> with out the brackets should properly install everything. (Under the assumption that pip is installed)

Instructions to Run:
1. For each .ipynb python notebook file (equal_weight_S&P_500_list.ipynb, momentum.ipynb, value.ipynb) run each cell within the file starting with the first cell to the last cell
2. Starting portfolio value can be modified for testing purposes by editing the "portfolio_size" variable

# Algorithmic Trading(Cluster)
To run this pyspark application in clustered mode on AWS:

1. Create s3 bucket: https://docs.aws.amazon.com/AmazonS3/latest/userguide/create-bucket-overview.html
2. Rename the {mypath} variable to the path of the s3 bucket: 's3://BUCKET-NAME/FILENAME.csv'
3. Create emr cluster: https://docs.aws.amazon.com/emr/latest/ManagementGuide/emr-setting-up.html
4. SSH into master node of emr using aws key_pair
5. pip install -r requirements
6. aws s3 cp 's3://BUCKET-NAME/FILE.py' .
7. spark-submit FILE.py
