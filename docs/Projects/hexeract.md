---
layout: default
title: Hexeract
parent: Projects
nav_order: 2
---

## Hexeract 

Hexeract is a fully systematic cloud based trading application. It encompasses:

    1) Data pipelines and WebSockets for high-frequency market data.
    2) Efficient data storage.
    3) Extract - transform - load of market data into signal generator. 
    4) A buy/sell signal generator.
    5) Portfolio manager/optimizer.
    6) Risk manager.

 

<p align="justify ">
 Code samples from the private repository are available <a href="https://github.com/jsingh-pb10/hexeract"> here</a>. The sampled code from the signal generator makes use of <a href="https://en.wikipedia.org/wiki/Dynamic_mode_decomposition"> Dynamic Mode Decomposition</a>. The sampled code from the portfolio optimizer makes use of hierarchal <a href="https://en.wikipedia.org/wiki/Risk_parity">risk parity</a>. This combination annually gives approximately 1.125 times the Nifty 50 annual return. Nifty 50 is a benchmark Indian stock market index that represents the weighted average of 50 of the largest Indian companies listed on the National Stock Exchange.
 </p>

<p align="justify ">
 Postscript: Hexeract was the core reason why I was able to finish Hudson at a very fast speed. For Hexeract I worked with a lot of satellite-derived geospatial data as it is useful for trading commodity derivatives, especially agriculture and energy-related ones. Thus I had good knowledge of how to efficiently work with huge amounts of spatial data which is the foundation of Hudson.
</p>