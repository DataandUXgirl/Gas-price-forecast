# Natural Gas Price Forecasting for Energy Trading

## Executive Summary:

The trading team at our energy investment firm relies on accurate natural gas price estimates to value storage contracts, execute seasonal trading strategies, and predict risk exposure. However, the desk only had monthly price snapshots, which made it difficult to model daily price movements or forecast future seasonal peaks.

Using Python, I transformed raw end of the month data into a continuous daily price curve and built a 12 month forecasting model. This allowed the trading desk to:

1. Understand natural gas seasonal patterns

2. Predict future winter vs. summer price cycles

3. Estimate daily price levels for PnL modeling

4. Improve contract valuation accuracy


From the analysis, I identified that:

1. Winter prices consistently peak 10% – 15% higher than summer lows, making winter the most profitable period for contract withdrawals.

2. Daily interpolation significantly improves pricing precision, especially for valuing optionality in storage contracts.

3. Future forecasts show elevated winter prices, suggesting traders should position inventory earlier.

These insights support better trading decisions, stronger pricing models, and improved long term gas trade strategy.

## Business Problem

Natural gas prices are highly seasonal, volatile, and sensitive to demand and supply shocks. For our trading desk, monthly price data made it difficult to:

1. Value long-term storage and transportation contracts

2. Estimate daily mark to market PnL

3. Develop seasonal trading strategies

4. Forecast future contract profitability

## Stakeholders asked:

### “How can we create reliable daily price estimates and forecast future prices to guide storage and trading decisions?”

This project solves that by building a daily interpolated price model, analyzing seasonality, and producing a 12-month price forecast to guide strategic positions.

*Original monthly price plot*

![Original monthly price plot](Monthly-natural-gas-prices.png)





## Methodology

1. Data extraction in python to load historical monthly natural gas prices
2. Visualization using matplotlib to visualize the monthly natural gas prices
3. Time series forecasting in Python (numpy) to interpolate daily prices and extrapolate future price trends
4. Visualization using matplotlib to visualize extrapolated future gas price trends

## Skills Demonstrated

- Python (Pandas, NumPy, Matplotlib), Time series modeling, Writing functions, statistics, Data Analysis, data visualization, finanacial modelling, Trend detection



## Results & Business Recommendations

By creating a daily price curve and forecasting future cycles, the trading desk gained full visibility into the seasonal nature of natural gas. Before this analysis, traders relied on monthly snapshots; now they can model day to day positions and optimize long term decisions.

*Extrapolated daily price curve 12 month forecast*


![Extrapolated daily price curve 12 month forecast](extrapolated_daily_gas_prices_12mo_forecast.png
)

## Key Findings

1. Natural gas shows a rise in price during the winter season about 10 - 15%, showing strong withdrawal opportunities.

2 During summer prices dip predictably, making it the best time for storage injections.

3. The forecast indicates the next winter may be slightly higher than previous years except 2024 winter, suggesting early positioning is beneficial.

4. Using the forecast model, traders can simulate multiple future scenarios to reduce pricing ris


Recommended Actions Based on the insights:

1. Lower average prices in June–August offer high value entry points which means storage injection should begin early in the summer
2. Sell structured products before winter peaks because predictable winter highs create profitable opportunities.
3. Incorporate forecast function in pricing models to improve contract valuation accuracy and reduces mispricing risk.
4. Consider Extending the Model by adding weather, demand data, seasons and henry hub fundamentals would increase forecasting reliability to help the trading team maximize returns and minimize risk.


## Next Steps

1. Build an automated daily price updater
2. Develop a dashboard for real time price monitoring with expanding the model to commodities like crude oil and propane
