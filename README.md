#**A module for a bot that trade the virtual currency automatically**
#####_Tested on Python 2.7.12_

### Features:
- predictionprice module is a set of tools for making the bot to automatically trade according to the prediction of rise or fall of the virtual currency tomorrow price.
- You can do mainly the followings by using this module.
  - To get the price of virtual currency from Poloniex.com
  - Prediction the rise or fall of tomorrow's virtual currency price by machine learning using the scikit-learn.
  - Implementation of the back test.
  - Optimization of the number of the features and training samples.
  - Implementation of the market trade with accessing to Poloniex.com in accordance with the predicted buying and selling signs.
  - Function to inform the results of the prediction and buying and selling by e-mail.

### Prerequired:
- [poloniex](https://github.com/s4w3d0ff/python-poloniex)>=0.1.2
- An account of Poloniex.com
- APIKey and Secret to access to Poloniex.com with API.
- A gmail account.

### Install:
```
git clone https://github.com/darden1/python-predictionprice.git
cd python-predictionprice
python setup.py install
```

### Uninstall:
```
pip uninstall predictionprice
```

### Usage:
- Open examples/predictionPriceBot.py and set your gmail address, password, poloniex.com APIKey and Secret.
- Run this script with nohup as following.
```
nohup python predictionPriceBot.py > out.log 2> err.log &
```
- You can check the process ID as following when you want to kill this process.
```
ps auxw | grep python
```
- You can change the combination of the currency you want to trade with `coins` and `basicCoin`.

###  Caution:
- It is **absolutely not guaranteed** to increase your assets by using this bot.
- I hope if this could help you to create a better bot. (I would be very happy if you would inform me when you could achieve it.)