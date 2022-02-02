# **Tradingview Sentiment Indicator**

Programming Language: Javascript

The indicator uses VWAP and volume profile to develop a market sentiment. Since PineScript does not have an option to use these indicators to build advanced algorithms, this code uses a workaround for this. It does this by the following

1. Create alerts for VWAP,SMA and Volume changes in Tradingview 
2. Tradingview sends these alerts to Gmail
3. Read the alerts from the Gmail, run the logic
4. Print the output onto Google Sheets

Output

The code outputs the following in real time based on the market

1. Strong Bullish: There is a strong bullish trend in the market
2. Weak Bullish: The trend is bullish but wait for additional signals or a confirmation
3. Strong bearish: There is a strong bullish trend in the market
4. Weak Bearish : The trend is bearish but wait for additional signals or a confirmation

