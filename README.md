# GOLD Scalper PRO MT5

This is a trading algorithm called GOLD Scalper PRO MT5, developed by Forex Robot Easy Team. It is designed to trade on the MetaTrader 5 platform. Please note that Forex Robot Easy is not the official developer of this product, but we are providing a sample code that can work as described in this product.

## Input Parameters
- LotSize: The lot size for each trade.
- StopLoss: The stop loss level in pips.
- TakeProfit: The take profit level in pips.

## Variables
- ticket: Order ticket number.
- buySignal: Flag for buy signal.
- sellSignal: Flag for sell signal.

## Entry Logic
The entry logic of this algorithm is as follows:
1. Get the current market impulse and correction using iMACD and iMA functions.
2. Check if the market impulse is positive and the correction is negative. If true, set buySignal flag to true.
3. Check if the market impulse is negative and the correction is positive. If true, set sellSignal flag to true.

## Exit Logic
The exit logic of this algorithm is as follows:
1. Check if there is an open buy position.
2. If the current price is below the stop loss level, close the buy position with stop loss.
3. If the current price is above the take profit level, close the buy position with take profit.
4. Check if there is an open sell position.
5. If the current price is above the stop loss level, close the sell position with stop loss.
6. If the current price is below the take profit level, close the sell position with take profit.

## Trading Algorithm
The trading algorithm is implemented in the OnTick() function:
1. Check if there are no open positions.
2. If true, generate entry logic.
3. If there is a buy signal, open a buy position with the specified lot size, stop loss, and take profit levels.
4. If there is a sell signal, open a sell position with the specified lot size, stop loss, and take profit levels.
5. If there are open positions, generate exit logic.

## Product Description
GOLD Scalper PRO MT5 is a trading algorithm developed by Forex Robot Easy Team. It is designed to trade on the MetaTrader 5 platform. The algorithm uses a combination of market impulse and correction indicators to determine buy and sell signals. The algorithm automatically opens and closes positions based on the specified lot size, stop loss, and take profit levels.

Please note that Forex Robot Easy is not the official developer of this product. We are only providing a sample code that can work as described in this product. To find the official developer of this product, please use MQL5.

For detailed reviews and trading results of this product, please visit [forexroboteasy.com/forex-robot-review/review-gold-scalper-pro-mt5-get-omega-trend-ea-as-a-gift/](https://forexroboteasy.com/forex-robot-review/review-gold-scalper-pro-mt5-get-omega-trend-ea-as-a-gift/)
