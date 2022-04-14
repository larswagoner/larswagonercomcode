+++ 
draft = false
date = 2022-01-30
title = "Deriving the Black-Scholes Formula"
description = "Black-Scholes"
slug = "black-scholes"
authors = ["Lars Wagoner"]
tags = ["Mathematics", "Finance", "Stochastic Modelling"]
categories = ["Projects"]
externalLink = ""
series = []
+++
In this project, we derive the Black-Scholes formula and apply it to real world options.
In order to tackle the challenge of anticipating the behavior of the option market, a
binomial model is obtained. The aforementioned model is the foundation upon which
the Black-Scholes formula for European option pricing is developed. At the end, an
analysis on the reliability of Black-Scholes will be implemented using real world data. 

*You can find the introduction below, contact me if you are interested in other parts of the paper!*



The financial world has always been an impactful actors in both the de-
velopment and decline of different cultures and societies. As one of the most important
elements of the financial market, the stock exchange and its ever-changing state have
been at the forefront of economic research.

The notion of a share can be simply described as the unit of ownership of a private
or public limited company. Depending on the type of company, shares can exist as fi-
nancial assets that allow the shareholder to benefit from the equal distribution of the
company’s profits, in the form of dividends. In the eventuality that companies do not
pay dividends, the shareholders can still trade their shares on the stock exchange.
Naturally, the price of a share can vary over time in accordance with the company’s
performance and forecasted profits. Although investing in shares can turn into a prof-
itable endeavour, the vast number of factors that influence their price makes it precarious.
One of the most employed ways of reducing the risks of share speculation is an option.
An option is a contract in which two parties enter into an agreement for a certain period
of time to; in principle, trade a certain underlying value at a predetermined price. In
the case of a stock option, this underlying value consists of shares. There are two types
of stock options: call options and put options.

A call option is the option buyer’s right to buy shares at a predetermined price during
the period of validity of the option contract. A put option is the option buyer’s right to
sell shares at a predetermined price during the period of validity of the option contract.
The period of validity of an option contract is called its term, the predetermined price
is called the strike price. If the option can be exercised any time during the term, it is
an American option. If the option can only be exercised at the end of the term on the
expiration date, it is a European option.

The trade in options takes place on an options exchange, with a standardization con-
cerning the contract size, generally of 100 shares; the term, typically of 3, 6, 9 or 12
months; and the expiration date of an option, the Saturday following the third Friday
of the month of expiration if the exchange is open on that day. It is also important to
note that an option can only be traded during its term.

Having established the benefits of option trading, the ability to anticipate the long-
term behaviour of the market is of great importance. Therefore, having the tools to
accurately approximate option prices becomes a great asset to the trader, making the
development of stochastic systems paramount. Consequently, the goal of the following
paper is to deduce and analyze the properties of the Black-Scholes (B-S) formula, based
on a binomial pricing model.
