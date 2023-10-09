**AUTOMATING CRYPTO WEBSITE API PULL PROJECT**

**Project Overview**

This portfolio project focuses on automating the retrieval of cryptocurrency data from the Coinmarketcap.com API, processing and visualizing the data, and conducting some basic analysis. The goal of this project is to create a script that pulls cryptocurrency data at regular intervals, stores it in a structured format, and generates visualizations and analysis.

**Code Description**

The project is implemented in Python and utilizes the requests library for API requests and pandas for data manipulation and analysis. My API key: a94b6406-c800-4cc5-b20d-6f790625c82e. Below is a breakdown of the code:

**Importing Libraries**

from requests import Request, Session

from requests.exceptions import ConnectionError, Timeout, TooManyRedirects

import json

import pandas as pd

import os

from time import time, sleep

import seaborn as sns

import matplotlib.pyplot as plt

**API Request and Data Retrieval**

• The script sends a GET request to the CoinMarketCap API to fetch the latest cryptocurrency listings.

• It handles potential connection errors and timeouts gracefully.

• The retrieved data is normalized into a Pandas DataFrame.

• The timestamp of the data retrieval is added to the DataFrame.

**Automating API Calls**

• The api_runner() function encapsulates the API call and data processing steps.

• A loop is used to call the api_runner() function at regular intervals (every 60 seconds in this case) for a specific number of times (333 in this case).

• The resulting data is continuously concatenated to create a comprehensive dataset.

**Data Analysis and Visualization**

• The script performs basic data analysis on the collected data, calculating the mean of specific percentage change values for each cryptocurrency.

• It then visualizes the percentage change values using a point plot.

• Additionally, it creates a line plot to track the price of Bitcoin over time.

**Data Storage**

The collected data is stored in a Pandas DataFrame (df) and continuously updated with each API call.

**Data Analysis**

The script calculates the mean of percentage change values for cryptocurrencies and creates visualizations to help understand trends over time.

**Dependencies**

requests

pandas

seaborn

matplotlib
