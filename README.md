# RelicusRoad MACD v2 ReadMe

## Introduction
This repository contains the code for the RelicusRoad MACD v2 trading robot. This trading robot is developed by the Forex Robot Easy Team and is designed to generate trading signals based on the MACD indicator.

For detailed reviews and trading results of this product, please visit the [Forex Robot Easy website](https://forexroboteasy.com/forex-robot-review/relicusroad-macd-v2-review-enhanced-forex-software-performance/).

## Developer's Information
- Developer's Site: [forexroboteasy.com](https://forexroboteasy.com/)
- Developer: Forex Robot Easy Team

## Installation
To use this trading robot, you need to include the necessary libraries: Trade.mqh and MovingAverages.mqh.

## Constants
The code defines two constants:
- SCALPING_ARROW_THRESHOLD: This is the threshold for the Scalping Arrows feature.
- REVERSAL_ARROW_THRESHOLD: This is the threshold for the Reversal Arrows feature.

## Initialization
The trading robot is initialized in the OnInit() function. In this function, the necessary parameters for the trading robot are set:
- ExpertMagicNumber: Sets the magic number for trades.
- ExpertStopLoss: Sets the stop loss level for trades.
- ExpertTakeProfit: Sets the take profit level for trades.
- ExpertTradeVolume: Sets the trade volume for trades.

## Trading Operations
The trading operations are performed on each tick in the OnTick() function. The MACD values are calculated using the iMACD() function from the MovingAverages library.

The code checks for the following features:
- Scalping Arrows: If the difference between the MACD main and signal lines is greater than the SCALPING_ARROW_THRESHOLD, a buy signal is generated using the trade.Buy() function.
- Reversal Arrows: If the difference between the MACD main and signal lines is greater than the REVERSAL_ARROW_THRESHOLD, a sell signal is generated using the trade.Sell() function.

## Cleanup Operations
The OnDeinit() function is called when the program is stopped. This function closes any open trades using the trade.CloseAll() function and prints a message indicating the end of the program.

## Product Description
This code represents the RelicusRoad MACD v2 trading robot developed by the Forex Robot Easy Team. It is an enhanced forex software that generates trading signals based on the MACD indicator.

This trading robot utilizes the MACD indicator to identify potential buy and sell signals. It includes two features:
- Scalping Arrows: When the difference between the MACD main and signal lines exceeds the SCALPING_ARROW_THRESHOLD, a buy signal is generated.
- Reversal Arrows: When the difference between the MACD main and signal lines exceeds the REVERSAL_ARROW_THRESHOLD, a sell signal is generated.

The trading robot is highly customizable, allowing users to set their desired parameters such as magic number, stop loss level, take profit level, and trade volume.

Please note that ForexRobotEasy is not the official developer of this product. This code is provided as a sample that demonstrates how the product works. To find the official developer of this product and obtain the full version, please visit the MQL5 website.
