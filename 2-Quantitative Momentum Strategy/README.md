## 2. Quantitative Momentum Strategy

The S&P 500 is the world's most popular stock market index. The largest fund that is benchmarked to this index is the SPDR® S&P 500® ETF Trust. It has more than US$250 billion of assets under management.

The project is a Python script that analyses the stocks in S&P 500 and selects top-50 stocks which have increased their price the most. This is called "Momentum-Strategy" where you only look at stocks which have a high price returns.

High-Momentum stocks were selected which had high one year, six month, three month, one month percent return metrics. Using the portfolio size from the user the script calcuates and gives you an excel-sheet with top-50 stocks you should invest in which have high-momentum.

I used an API from IEX which gave me data related to a company's stock metrics like latest price, market capital, change percentage, etc. I have used a free API which did not gave me the true values for all these metrics but they were very close to the real values with an error of +-5 units.

I implemented batch-API calls and divited my 505 stocks in groups of 100 each so as to use batch-api version of IEX CLoud API. This made my API calls way faster rather than doing separate calls for every 505 stocks.
