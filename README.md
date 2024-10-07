# Netflix Stock Price Analysis

## Objective

The analysis aimed to model and forecast Netflix's stock price using the ARIMA model.

## Data Overview

The data utilized consists of Netflix's historical stock prices, specifically focusing on the adjusted closing prices. The dataset was divided into training and testing sets, with 80% of the data used for training the ARIMA model and 20% for testing.

## Model Used

An ARIMA (1, 1, 1) model was employed to capture the underlying patterns in the differenced stock prices. The first differencing of the stock prices was used to ensure stationarity.

- Training Set: The ARIMA model was fitted on differenced training data consisting of 80% of the dataset.
- Testing Set: The model was used to forecast on the testing data to compare the actual vs predicted values.

## Key Findings

### Model Diagnosis

Upon diagnosing the ARIMA model, increasing volatility in the residuals over time was observed, particularly after 2014. This indicates that ARIMA might struggle to capture the volatility present in Netflix's stock price.

### Residual Analysis

The residuals exhibited fat tails, which indicates large errors in the model, suggesting that the ARIMA model may not capture the extreme price fluctuations effectively. The residuals were also not normally distributed, violating a key assumption of the ARIMA model.

### Post-COVID Market Corrections

The COVID-19 pandemic significantly impacted Netflix’s stock price as a rapid increase in subscribers led to a rise in stock prices during the lockdown period. However, post-pandemic, as lockdowns eased and consumer behavior shifted, market corrections became apparent.

## Future Work to Improve the Model

To further enhance the accuracy and robustness of the Netflix stock price model, incorporating additional macroeconomic factors that directly influence consumer behavior and market conditions is recommended. Future work could involve integrating the following factors into the model:

- **Consumer Confidence**: By incorporating consumer confidence data, the model can better capture changes in discretionary spending on services like Netflix, which directly impacts subscription growth and churn rates.
- **Disposable Personal Income**: Including this factor would allow the model to account for fluctuations in household income, particularly as economic conditions shift, impacting consumers’ ability to afford non-essential services like streaming subscriptions.
- **Inflation and Interest Rate**: Post-pandemic, rising inflation and interest rates have altered consumer spending power and increased operating costs for companies like Netflix. Incorporating these factors into the model would allow for a better understanding of how macroeconomic pressures influence stock price movements.
- **Market Volatility**: Netflix's stock price is highly sensitive to broader market movements. Incorporating market volatility indicators, such as the VIX index, could help the model capture periods of heightened uncertainty and better account for price fluctuations.

By integrating these macroeconomic factors, segmenting the data into pre- and post-COVID periods, and considering advanced models like GARCH or VARMAX to handle volatility, the model could better reflect real-world conditions and provide more accurate forecasts for Netflix's stock price.




