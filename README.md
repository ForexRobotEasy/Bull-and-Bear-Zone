# Bull and Bear Zone Indicator

This is a custom indicator developed by Forex Robot Easy Team, available at [forexroboteasy.com](https://forexroboteasy.com). The Bull and Bear Zone Indicator is a minimalist trading indicator designed for both manual and algorithmic trading upgrades.

## Indicator Initialization

The initialization function `OnInit()` is called when the indicator is attached to a chart. In this function, the indicator buffer mapping is set using `SetIndexBuffer()`. Two buffers are used, `BullZoneBuffer` and `BearZoneBuffer`, each representing the Bull Zone and Bear Zone lines respectively. The indicator line settings are configured using `SetIndexStyle()` and `SetIndexLabel()` to specify line styles and labels for each buffer. The `IndicatorDigits()` function is used to set the number of digits displayed on the chart based on the market information. The initialization function returns `INIT_SUCCEEDED` to indicate successful initialization.

## Indicator Calculation

The calculation function `OnCalculate()` is called for each new tick of data. It receives arrays of price data, including `time[]`, `open[]`, `high[]`, `low[]`, and `close[]`. The function also receives arrays for tick volume, volume, and spread. The function calculates the Bull and Bear zones using a loop that iterates over the new data points.

For each data point, the function compares the high and low prices with the previous Bull Zone and Bear Zone values. If the high price is higher than the previous Bull Zone value, the Bull Zone value is updated with the new high price. Otherwise, it retains the previous Bull Zone value. Similarly, if the low price is lower than the previous Bear Zone value, the Bear Zone value is updated with the new low price. Otherwise, it retains the previous Bear Zone value.

The function returns the total number of rates calculated, which is equal to `rates_total`.

## Product Description

The Bull and Bear Zone Indicator is a powerful trading tool developed by Forex Robot Easy Team. It provides traders with a minimalist and effective way to identify Bull and Bear zones in the market. This indicator can be used for both manual trading and algorithmic upgrades.

The indicator works by calculating the Bull and Bear zones based on price data. The Bull Zone represents the maximum high prices observed, while the Bear Zone represents the minimum low prices observed. By identifying these zones, traders can gain insights into market trends and make informed trading decisions.

The Bull and Bear Zone Indicator is designed to be easy to use and understand. It provides clear lines on the chart that represent the Bull and Bear zones. Traders can use these lines as support and resistance levels or as entry and exit points for their trades.

Please note that Forex Robot Easy is not the official developer of this product. We are showcasing this sample code that demonstrates how the indicator works. To find the official developer of this product and access detailed reviews and trading results, please visit [forexroboteasy.com](https://forexroboteasy.com/forex-robot-review/bull-and-bear-zone-forex-software-review-a-minimalist-trading-indicator-for-manual-and-algorithmic-upgrades/).

For detailed reviews and trading results of this product, please visit [forexroboteasy.com](https://forexroboteasy.com/forex-robot-review/bull-and-bear-zone-forex-software-review-a-minimalist-trading-indicator-for-manual-and-algorithmic-upgrades/).
