---
layout: post
title:  "How to exploit people's lack of patience"
date:   2023-10-26
categories: manifold
---

# Background

The October 2023 Speaker of the House market was a perfect opportunity to earn some (real or fake) money. You could try front-running the news based on some form of sentiment analysis. Or you could exploit Manifold's website lag in trade execution through the API.


But of course, we need more. We assume that the market will revert to its true cost after a large order is placed. This is either a correct assumption, in which our bot places a bet against that order.
Or this is an incorrect assumption. Which is why a delay is needed before confirming the trade. Only make the trade after a set duration with no large trades in that direction.


# How to not lose money and not make bad bets

Use limit orders. Use common sense.

# How to win

Now automate this, and you have [Michael's bot](https://github.com/mwhea/Manifold_Trading_Bots) but worse? Coming soon.