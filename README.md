# gold_price_forecast

We used the following macroeconomic indicators to build a forecast model for Gold:
- Gold
- USInf (US Inflation index)
- DollarIndex
- FedFundRate (Fed Fund Rate)
- SPX (SPX Index)
- Vix
- Govt10 (10-year Government Bond Yield)
- Govt2 (2-year Government Bond Yield)
- Unemployment

Additionally, we included some derived data, such as 5-day and 20-day changes in some of the above factors, to provide the model with a sense of change, as changes are significant drivers of prices.

Our neural network model had 25 input nodes, 2 hidden layers of size 300, and an output layer of 3. For the output layer, we used the sigmoid activation function and ReLU elsewhere.

Conclusion:
The Gold forecast model shows a better Sharpe ratio than simply being long in Gold. However, further work is needed, and various combinations of input features need to be explored.

I would also like to try less black box models like random forests to see if I can achieve similar or even better results.

Hopefully, one day, I will find that holy grail of a model, become rich, and be able to retire. Sigh...

One interesting observation is that the function shows some jumps when major events happen, creating short-term trading opportunities.

The output level of the sigmoid function provides a conviction level, and it's intriguing to see that when short-term conviction jumps, the price tends to follow. However, more evidence is needed. Overall, the results are satisfactory but not mind-blowing.
