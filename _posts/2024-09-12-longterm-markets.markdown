---
layout: post
title:  Problems and Solutions to Long term Prediction Markets
date:   2024-09-02
---
# Long term forecasting and prediction markets


If you were to visit Manifold about a year ago, you would have noticed [a market that claimed AI had a 30% chance of wiping out humanity before 2030](https://manifold.markets/MartinRandall/will-ai-wipe-out-humanity-before-th-d8733b2114a8) or a 4% chance of aliens being real. This incredulous market, however, was distorted by fundamental issues with long term prediction markets. 

Long term markets suffer from locking up capital without obtaining interest. The opportunity cost of the locked up capital is quite massive over a time horizon of many years. Recent attempts to pay interest on predictions are unlikely to encourage long term forecasts. Interactive Brokers’ (IBKR) event contracts pays the Federal Funds rate at the current value of the position, minus 50 basis points. Compounded over 10 years, that means that one requires an edge of ~20% compared to traditional investments.

Platforms that offer long-term real money prediction markets, such as Kalshi and IBKR, see these markets as having quite low liquidity and interest as a result. [A Kalshi market resolving in 2030 has only a few thousand in volume traded and resting orders, not useful for any serious trader or person needing to hedge risk.](https://kalshi.com/markets/chinausgdp/china-overtakes-us-gdp)

Forecasting platforms like Metaculus and GJOpen rely on expert predictions, however, their algorithms are often opaque and slow to update. [Although, Metaculus is going open source soon.](https://www.metaculus.com/notebooks/25078/open-sourcing-metaculus/)

I’m an economic advisor and developer at [PlayMoney](https://playmoney.dev), a completely play-money and open source prediction market. Designing economies that incentivize accurate predictions are hard, and we need to get the economy right to make sure users are incentivized to participate and enjoy forecasting.

But first we need some metrics to measure the economy. Calculating the interest rate on prediction markets is not straightforward. [We could naively make a bond market that is guaranteed to resolve at a certain date.](We could naively make a bond market that is guaranteed to resolve at a certain date.) But this approach is flawed, as no user is willing to bet against you, forcing a participant to either continue to fight the capital or take paper losses (quite harmful if one obtains interest or a loan based on the value of the position). In fact, large asymmetric capital requirements between YES and NO bettors, such as [the infamous UFO market.](https://manifold.markets/Joshua/will-eliezer-yudkowsky-win-his-1500) If a market is trading at 2%, that means a NO holder needs 50 times more capital as any YES holder. Such an asymmetry is clearly a massive issue for any NO holder (usually a sharp whale) compared to the YES holder (the eccentric UFO truther).

These long-term markets are often compared to a “stonk”. A stonk on Manifold Markets is a market with no intrinsic value, which never resolves and pays out. The only way to reliably profit is to anticipate how other traders will trade, similar to a [Keynesian Beauty Contest.](https://en.wikipedia.org/wiki/Keynesian_beauty_contest) Many traders on Manifold note that the behavior exhibited by stonks are similar to meme stocks or meme coins with little intrinsic value, rather, trading based on popularity. The [Did Covid-19 Come From A Lab market](https://manifold.markets/IsaacKing/did-covid19-come-from-a-laboratory) is often highly reactive to whatever Peter Miller or some other whales or minnows think at any given moment, and not reflective of actual realities. In fact, since disproving something (in this case, that Covid-19 did not come from a lab) happened is often impossible, the market could possibly never resolve, indeed turning the market into a stonk.

So, how does PlayMoney plan to accurately incentivize long-term predictions? We make a few assumptions to simplify this problem.

First, that more skilled predictors or market participants have orders of magnitude, or at least Pareto amounts of capital (in markets) or weight (in forecasting platforms). Secondly, that skill in forecasting near term events correlates with forecasting long term events. This hypothesis is tentatively true, as noted in the decades long tournament from Tetlock’s Superforecasting. Finally, we assume that markets are well calibrated in the near term.

Using a purely reputation-based points system avoids capital lock up while also giving incentives to be correct in the near term. The amount of weight given to a certain user depends on both their points from long-term predictions and currency. 
Aggregation of points will be done in a decaying format, or possibly, users may be given short-term incentives to make long-term forecasts.

These methods are mostly the same as Metaculus. The real innovation comes from the tie-in to an actual vibrant economy, which we hope will draw in many new users while giving valid, accurate predictions. 

