Plotly Presentation
========================================================
author: Afsah
date: 10/6/2020
autosize: true


Introduction
========================================================

Plotly and RMarkdown Presentation

This is for the peer assessed assignment at Coursera.



Codes in Creating Plotly
========================================================


```r
library(plotly)
library(tidyr)
library(dplyr)
data("EuStockMarkets")
stocks <- as.data.frame(EuStockMarkets) %>%
  gather(index, price) %>%
  mutate(time = rep(time(EuStockMarkets), 4))
plot_ly(stocks, x = ~time, y = ~price, color = ~index, mode = "lines")
```

Plot
========================================================



```
Error in loadNamespace(name) : there is no package called 'webshot'
```
