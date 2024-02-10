# DeFi-DIY: Ranged Limit Orders
##### *Of all trading and earning tools users look for in any DeFi platform, the most sought-after feature is limit orders.*
---

#### :zap:Using Osmosis' *Concentrated Liquidity* to make easy, slippage-free limit orders:zap:

Unlike using a *CEX*, automated trades in DeFi traditionally involve *smart contracts*. This can be confusing or intimidating to some users, and depending on the chain or the trading platform aren't always an option. 
They also might behave differently then expected, especially to those accustomed to trading by *CEX*. Normally swaps will happen at the target you set, but price accuracy and swap reliability could be questionable, since slippage and price effect still apply.
> :exclamation:In extreme cases, such as during rapid price swings combined with severe network congestion, some contract-based limit orders may fail to execute at all.

Luckily, due to how *Supercharged Liquidity* pools work, by creating a specific kind of position you can mimic **true** limit orders right on *Osmosis* in just a few seconds. :point_down:Here's how:point_down:
 
 ---
 <br>
 
In short, find a pool for the pair you want to swap, choose your price point, and finally create a position where *both low and high* price range points are just a tiny fraction above, or below your target price. Which side of your target price to place your range is determined by which of the pair in that pool you are looking to sell.
<br>

---
![image](https://hackmd.io/_uploads/H1tmmamsp.png)

---

> :point_up:*Looking at the pool above, assume you want to sell DYM at a price of 7.47USDC*:point_up:


To make a *limit-sell* order in pool [#1450 DYM/USDC](https://app.osmosis.zone/pool/1450), set both upper *and* lower range points just above your sell price of 7.47.
After you create a position, if DYM price moves in your favor it will begin converting to USDC. When it crosses the target price, the position is fully converted to USDC and can be removed. 

:memo:You can use many decimals - the closer to target price it is (without going past) the closer to quote (`tokenAmount*tokenPrice`) you get in the end.

<br>

---

![image](https://hackmd.io/_uploads/rkdtETXip.png)

---
> :point_up:*Shown above, making a *limit-buy* order for the same pool is just as easy.*:point_up:

##### :memo: Remember, the goal is changing the expected deposit to a single asset - the one you want to sell.

This time, by placing the range limits anywhere below current market price, the expected deposit is 100% USDC. 
If you want to wait for a discount and get DYM at 7.00USDC, set these points around 6.99 and 6.999, and just like before the USDC converts to DYM as the price moves toward your target. When complete, you will have paid an average price very near to 7.00USDC.

:exclamation:Remove the position as soon as possible! If you leave it, the price could swing the other way and end up swapping back.

<br>

:zap: **In addition**, while your narrow position is *in range*, you will earn from swap fees and incentives (where applicable) from the pool!
<br><br><br><br><br>

###### p.s. Quickly + easily check Osmosis pools for incentives using  [@Cosmos_Directory_Bot](https://t.me/Cosmos_Directory_bot) on Telegram!

<br>


###### *Thanks to Robo for inspiring this writeup*[^1]. *Twice for repeated/last-minute proofreading & feedback.*
[^1]: @RoboMcGobo Osmosis CL Pool Limit-Order trick [twitter thread](https://twitter.com/RoboMcGobo/status/1755028750926786753).
.
