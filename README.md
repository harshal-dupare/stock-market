# stock-market

## Check the following
+ Refer UML folder for use cases & overall package relation
+ Are there anyother use cases ?


## data 
Contains data that can be accessed by a strategy, and code to get data from different sources e.g. quandl


## microstructure
Contains all the modules/packages for defining the structure and functionality of market E.g. 
  * Order : types of orders and their functionality like canceling an order etc.
  * Market : how orders are executed // will be useful when making live simulations
  * Can make different players in the market to add when used in simulations : e.g. Brokers, Sell side, Buy side, Invester with multiple strategies.
  
## strategy
Contains various codes for differnt strategy and general skeleton of a strategy

* Each startegy takes in input of timely data/updates and output a set of timely orders


## backtester
Contains core backtesting class with different metrics
* Input of data & strategy
* Output Results with specified metrics + default ones

## simulator 
Contains different simulator class with different type of model of the market (either on order books / or just OHLCV data)
* Each will have same and consistant format for input
