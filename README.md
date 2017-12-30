#Stock data visualisation and analysis in R

This repository contains test codes to access, visualise and analyse ASX stock data in R.

## Packages used

* quantmod

## Get ASX listed stock practices

Get Woolies (WOW) stock from Yahoo and create candlestick chart.

```r
require(quantmod)
getSymbols("WOW.AX", src="yahoo")
barChart(WOW.AX, subset='2017-1::2017-11')
candleChart(WOW.AX, subset='2017-9::2017-12',
            up.col='yellowgreen',dn.col='orangered2')
addBBands()
```

## Shiny app demo

## References
