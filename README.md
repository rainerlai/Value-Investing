# Value-Investing
Developing an investment strategy using information signals to generate alpha returns

--------------------------------------------------------------------------------------------------
*Note
The company stock data file taken from WRDS is split into batches due to file size limit

The following python code us used to chunk the file into uploadable file sizes for the repository 

import pandas as pd
source_path = r"...\company_stock_1999-2021.csv"
for i,chunk in enumerate(pd.read_csv(source_path, chunksize=700000)):
    chunk.to_csv(r'...\chunk{}.csv'.format(i), index=False)
    
---------------------------------------------------------------------------------------------------

To develop an investment strategy using relevant information signals (including accounting information from financial statements) that can generate alpha returns.

Using the tradeable universe of U.S. companies excluding all banks and financial institutions using 15 years of relevant data, ending not earlier than 2020

Employing accounting data from financial statements as information signals and using other non-accounting data such as momentum factor.
Data sources includes Compustat, CRSP, Bloomberg, Capital IQ, Yahoo Finance. H
Using monthly stock price/return data and annual financial data to assess the profitability of the investment strategy using the following investment performance measures: 
(i) raw return, (ii) Sharpe ratio, and (iii) maximum drawdown.
