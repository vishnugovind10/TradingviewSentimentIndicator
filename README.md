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

The algortihm calculates the market sentiment over several time periods. It then aggregates all these time periods to build a market color. 

  A strong trend is when the short term market direction agrees with the long term and vice versa
  
  Based on the above signals several strategies can be devised
  
  1. Swing Trading: Jump in on the trade at the beginning of a trend (when short term and long term trends agree)
  2. Scalping: Trade the short term and exit for a quick profit ( this can be used when short term and long term trends do not agree)
