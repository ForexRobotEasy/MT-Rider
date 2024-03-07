# MT Rider Expert Advisor

MT Rider is an Expert Advisor developed by forexroboteasy.com. It is designed to identify and trade multi-timeframe Forex trends using the Moving Average Convergence Divergence (MACD) indicator. This code serves as a sample implementation of the MT Rider strategy.

For detailed reviews and trading results of the official MT Rider product, please visit the following link: [MT Rider Review - Unveiling Multi-Timeframe Forex Trends](https://forexroboteasy.com/forex-robot-review/mt-rider-review-unveiling-multi-timeframe-forex-trends/)

**Disclaimer: ForexRobotEasy is not the official developer of the MT Rider Expert Advisor. We only provide this sample code to demonstrate the concept behind the product. To find the official developer of the MT Rider Expert Advisor, please refer to MQL5.**

## Indicator Files

The code includes the following indicator files:

- MovingAverages.mqh
- MACD.mqh

These indicators are necessary for the calculation of the MACD values.

## Global Variables

The following global variables are declared:

- `fastEmaPeriod` (int): Period for fast Exponential Moving Average (EMA) calculation.
- `slowEmaPeriod` (int): Period for slow EMA calculation.
- `signalPeriod` (int): Period for signal line calculation.

## Initialization Function

The `OnInit` function is responsible for initializing the Expert Advisor. It performs the following tasks:

- Initializes the MACD indicator using the current symbol and timeframe.
- Enables the display of all time intervals simultaneously on the chart.

## Deinitialization Function

The `OnDeinit` function is called when the Expert Advisor is being removed from the chart. It cleans up and removes the MACD indicator.

## Start Function

The `OnTick` function is the main entry point for the Expert Advisor. It is executed on every tick of the market. The function performs the following tasks:

- Calculates the MACD values using the MACDOnArray function.
- Determines the trend direction by analyzing the histogram values.
- Calculates the trend average in percentages.
- Displays the trend average using the Comment function.
- Executes trading functions based on the identified trend direction.

Please note that the code provided here is a simplified version for demonstration purposes. The actual MT Rider Expert Advisor may have additional features and logic.

For more information about the official MT Rider Expert Advisor, please refer to MQL5 and visit the provided link for detailed reviews and trading results.
