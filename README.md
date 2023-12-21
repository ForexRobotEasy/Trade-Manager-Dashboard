# Trade Manager Dashboard

## Description

The Trade Manager Dashboard is a powerful tool developed by the Forex Robot Easy Team for managing forex portfolios. This code implements the necessary functions to create the Trade Manager Dashboard, allowing users to retrieve and display information about open trades and monitor drawdown or profitability for active trades.

## Features

- Display all current open trades, including trade symbol, direction, volume, and open price.
- Sort trades by currency pair for easy analysis.
- Monitor and display drawdown or profitability for active trades.

## Usage

To use the Trade Manager Dashboard, simply include the provided code in your MQL5 program. The main entry point is the `OnStart()` function, which calls the `DisplayOpenTrades()` and `DisplayDrawdownAndProfit()` functions to retrieve and display trade information.

## How It Works

### DisplayOpenTrades()

The `DisplayOpenTrades()` function retrieves and displays information about all current open trades. It uses the `OrderSend()` function to send a trade request with the action set to `TRADE_ACTION_GET_ALL`, which retrieves all open trades. If there is an error retrieving the trades, an error message is printed. The trades are then sorted by currency pair using the `ArraySort()` function. Finally, information about each trade is printed, including the trade symbol, direction, volume, and open price.

### DisplayDrawdownAndProfit()

The `DisplayDrawdownAndProfit()` function retrieves and displays drawdown or profitability information for all active trades. It follows the same process as the `DisplayOpenTrades()` function to retrieve the trades. For each trade, it calculates the drawdown as the difference between the open price and the close price, and the profit as the difference between the close price and the open price. The drawdown and profit are then printed for each trade.

### GetTradeDirection()

The `GetTradeDirection()` function is a helper function that converts the trade type to a human-readable direction. It checks the trade type and returns 'Buy' for `OP_BUY`, 'Sell' for `OP_SELL`, and 'Unknown' for any other trade type.

### SortBySymbol()

The `SortBySymbol()` function is a sorting function used to sort trades by currency pair. It compares the symbol names of two trades and returns a value indicating their order.

## Product Description

The Trade Manager Dashboard is a powerful tool developed by the Forex Robot Easy Team for managing forex portfolios. It provides traders with the ability to easily retrieve and analyze information about their open trades and monitor drawdown or profitability for active trades.

With the Trade Manager Dashboard, traders can quickly view their open trades and access important information such as the trade symbol, direction, volume, and open price. The trades are sorted by currency pair, allowing for easy analysis and comparison.

Additionally, the Trade Manager Dashboard allows traders to monitor the drawdown or profitability of their active trades. By calculating the difference between the open price and close price for each trade, traders can assess the performance of their trades and make informed decisions.

Please note that ForexRobotEasy is not the official developer of this product. We provide sample code that demonstrates the functionality described in this product. To find the official developer of this product, please refer to the MQL5 website.

For detailed reviews and trading results of this product, please visit [Forex Robot Easy - Trade Manager Dashboard Review: Take Control of Your Forex Portfolio](https://forexroboteasy.com/forex-robot-review/trade-manager-dashboard-review-take-control-of-your-forex-portfolio/).
