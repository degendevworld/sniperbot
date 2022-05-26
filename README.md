
## HOW TO RUN
1. clone this repository
2. $ npm install
3. Edit your <code>env.json</code>


```js
RPC = //your NODE url. Use the default BSC Dataseed to test it. if a custom node or ETH. Custom nodes are way faster but if you want, you can use free services for BSC nodes like Infuria / Moralis / Quicknode or Binance nodes. For Eth you can also use the same or https://ethereumnodes.com/

CHAIN = //the Chain of your target network such as 56 for BSC, 1 for ETH etc.

RECIPIENT = //Your address to receive tokens at

PRIVATE_KEY = //Your private key to sign the transaction

CONTRACT_TO_SNIPE = //The target contract address you want to snipe

MULTIPLIER: = //How many transactions to submit, ie buy 1 time or 5 times etc

GAS_LIMIT: = //best to leave it at default 1000000

AMOUNT_TO_BUY = //amount in either ETHER or BNB to buy depending on your NODE, accepts decimals

PROFITPERCENT= //profit to take which will initiate a sell

STOPLOSSPERCENT = //loss at which to initiate a sell

percentOfTokensToSellProfit= //sell % when profit is reached

percentOfTokensToSellLoss = //sell % when stoploss is reached

trailingStopLossPercent= //% trailing stoploss

maxLiquiditymax = //max Liquidity in BNB the contract needs to have for the buy to initiate

minLiquidity = //min Liquidity in BNB the contract needs to have for the buy to initiate

```

6. run with <code>node bot.js </code>.

7. Wait the bot do his job
   


## TROUBLESHOOT
* there are some reason if your tx failed :
- you haven't approve your BNB
- your gas price are to small
- your GWEI are to small (use 15+ for early token)
- your slippage are to small (use 30+ for early token)

![advanced](https://user-images.githubusercontent.com/105888892/169407294-509687df-632d-452d-a3c1-339fe2b065b7.png)
