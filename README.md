# Stock Market Trends and Price Prediction

#### MACHINE LEARNING


AAYUSH NEELKANTH  aayush27_soe@jnu.ac.in
BHAVISHYA RAJ  bhavis58_soe@jnu.ac.in <br>
JATIN VERMA  jatin71_soe@jnu.ac.in <br>
PEEHOO JAIN  peehoo78_soe@jnu.ac.in <br>
R SHRAVAN  shrava72_soe@jnu.ac.in <br>


## DESCRIPTION

The prediction process of stock values is always a challenging problem because of its unpredictable nature. The dated market hypothesis believed that it was impossible to predict stock values and that stocks behave randomly, but recent technical analyses show that the most stocks values are reflected in previous records, therefore the movement trends are vital to predict values effectively. Moreover, stock market groups and movements are affected by several economic factors such as political events, general economic conditions, commodity price index, investors’ expectations, movements of other stock markets, the psychology of investors, etc. The value of stock groups is computed with high market capitalization. There are different technical parameters to obtain statistical data from the value of stock prices. Generally, stock indices are gained from prices of stocks with high market investment and they often give an estimation of the economic status in each country. For example, findings prove that economic growth in countries is positively impacted by the stock market capitalization.

<a href = "https://www.kaggle.com/borismarjanovic/price-volume-data-for-all-us-stocks-etfs"><h4>DATASET DESCRIPTION</h4> </a>

Data is presented in txt format that we will convert it into a csv file. It includes attributes such as Date, Open, High, Low, Close, Volume, OpenInt. A lot of Ups and Downs in the value of Stocks and ETFs are present in the Dataset therefore we have a very wide variety of Database which we will perform to train and test our Model.

## MOTIVATION

Stock price prediction is a classic and important problem. With a successful model for stock prediction, we can gain insight into market behaviour over time, spotting trends that would otherwise not have been noticed. With the increased computational power of the computer, machine learning will be an efficient method to solve this problem.

We will introduce a framework in which we integrate user predictions into the current machine learning algorithm using public historical data to improve our results. The motivating idea is that, if we know all information about today's stock trading (of all specific traders), the price is predictable. Thus, if we can obtain just partial information, we can expect to improve the current prediction lot. With the growth of the Internet, social networks, and online social interactions, getting daily user predictions is a feasible job. Thus, our motivation is to design a public service incorporating historical data and users’ predictions to make a stronger model that will benefit everyone.


## CHALLENGES

Predicting stock price with 100% accuracy is almost impossible in reality as the stock price is heavily influenced by unquantifiable factors, such as market irrational behaviour and news.

These external factors can affect the stock market, thus affect our model:

- Supply and demand. For example, if traders tend to buy this stock more than selling it, this will affect the price probably by rising since the demand will be more than the supply.
- Stock prices can have unexpected moves because of single news which keeps a stock artificially high or low. Hence, investors cannot predict what will happen with stock on a day-to-day basis. This is called market sentiment factors and they include company news, economy, and world events.
- Global economy. The flow of money and transactions is based on the economy of the traders which is affected by the economy of the country. Stock historical prices. Each stock has a range in which tick data moves within when looking into chart patterns and behaviour of investors.
- Public sentiments and social media. A tweet from a president or an article release affects the price of the related stock(s). For example, an unofficial resignation of a CEO on Twitter.
- Natural disasters. For example, the “Haiti earthquake” that killed around 316,000 people affected the S&P index by going down 6.6% after 18 trading days.
- Earnings per share (EPS) is a fundamental factor that affects stock price. Investors tend to purchase stocks with high EPS since they know that they will gain substantial profits. The demand for this stock, the company management, the market sector dominance, and the cyclical industry performance result in the movement of the stock price.
- Inflation and deflation are technical factors. Inflation means higher buy price and thus higher interest rates. This will result in a decrease in stock price. On the contrary, deflation means lower buy prices and thus lower profits and interest rates.

There were various other problems as well:

- We had a lesser knowledge of various finance-study based models, like OU GARCH etc.
- There were a lot of methods, to solve this problem and finding the best suited one is quite a challenge
- The innate unpredictability of stocks and EFTs.


## METHODOLOGY

#### ARIMA MODEL

ARIMA stands for Auto-Regressive Integrated Moving Averages. AIMA(p,d,q) is a generalization of an autoregressive moving average (ARIMA(p,q)) model. ARIMA models are applied in some cases where data show evidence of non-stationarity. The AR term p of ARIMA indicates that the evolving variable of interest is regressed on its own lagged (i.e., prior) values. The MA part indicates that the regression error is a linear combination of error terms whose values occurred contemporaneously and at various times in the past. The I (for "integrated") indicates that the data values have been replaced with the difference between their values and the previous values (and this differencing process may have been performed more than once)

As the autocorrelation lag plot of stock, closely follows a straight line. Its distribution looks normal. Both plots suggest that ARIMA would be a good model for the data.

#### XGBoost MODEL

XGBoost stands for “Extreme Gradient Boosting”, where the term “Gradient Boosting” originates from the paper Greedy Function Approximation: A Gradient Boosting Machine, by Friedman. XGBoost is used for supervised learning problems, where we use the training data (with multiple features) to predict a target variable.

Gradient boosting is a process to convert weak learners to strong learners, in an iterative fashion. According to Friedman’s gradient boosting algorithm, on each iteration, the gradient descent is first computed to fit a new base learner function. Once the best gradient descent step direction and size are found, the function estimation is updated. Gradient boosting is an approach where new models are created that predict the residuals or errors of prior models and then added together to make the final prediction. It is called gradient boosting because it uses a gradient descent algorithm to minimize the loss when adding new models.

Three main forms of gradient boosting are supported:

- Gradient Boosting algorithm is also called a gradient boosting machine including the learning rate.
- Stochastic Gradient Boosting with sub-sampling at the row, column, and column per split levels.
- Regularized Gradient Boosting with both L1 and L2 regularization.

```
▪The End
```
