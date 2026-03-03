Overview

	This project is a custom multi-component indicator developed in Pine Script v5 and executed on 
	the TradingView platform. It combines statistical smoothing, volatility adjustments, and 
	specified logic into a single stock indicator. 

      The system integrates the following:
		- Gaussian-Weighted Smoothing Channel
    	- Dynamic Volatility-Based Bands
    	- Moving Average Engine
    	- Mean-Reversion Trigger Detection
    	- Buy/Sell Signal Labels
    	- Alert Conditions
      
	The combination for several components strengthens the assertions and reveals patterns. 
	This indicator is designed primarily for day trading and trend filtering for potential investors. 

Implantation

    Gaussian-Weighted Smoothing Channel: Applies higher weight to recent price data and 
	    gradually reduces the weight for older bars
    
    Dynamic Volatility-Based Bands: Derived from the Gaussian output, Mean Absolute Error, and 
    	a defined multiplier to reveal the breakout detection zones
    
    Moving Average Engine: Combination of Modified Hull MA, Hull MA, Exponential MA, Weighted MA, 
    	Volume Weighted MA, Simple MA, and RMA
    
    Mean-Reversion Trigger Detection: Plots a signal when the previous 5-minute candle closes 
    	beyond either band and the current candle is bullish

Development

	The indicator was built as a combination of several strong existing indicators that were adapted 
	to work in combination. It uses custom Gaussian channels as well as arrays for historical 
	weighted calculations that provide intraday filtering logic.
