# machine-learning-for-signal-in-FX-market
Data is extracted from fxcmpy, a database and virtual FX trading app. 

I extract the nanosecond change of big and ask price for EUR/USD.

Letting midprice to be the middle of ask and bid price for an interval 5 minutes. Then I get the 5-minute return from midprice. 

Moreover, since FX market does not have many alpha factors. we can let lag1,lag2,lag3, lag4, lag5 to be factors 
because we can assume price in certain time before may influence the price of FX market.

Using returns as signal of increasing or decreasing, we can separate data into two class and using many machine learning strategy to analyze.

Here, I use SVM, AdaBoost, random forest, extra tree, gradient boost to test which one is better.
