You may be familiar with the term 'slippage' from other DEXes. Often people will say to 'increase slippage' to get a trade to go through. But what does this actually mean, and is 'price impact' actually the same?

They both relate to the output you receive from a trade, but they are not both controllable by you as the trader. 

Price impact is most noticeable in pools with low liquidity. It is easiest to explain these two terms with visuals from the DEX. We will look at a high-liquidity pool and then one with low liquidity. 

Heading to [app.osmosis.zone/pools ](https://app.osmosis.zone/pools)and sorting the pools by total liquidity, we see that the ATOM/OSMO pool, [pool 1](https://app.osmosis.zone/pool/1), has the most liquidity on the whole DEX. Let's simulate a trade there.

![](https://i.imgur.com/SRe0nTg.png)

On the pool's page, click on the Trade Pair button at the top. It will open the swap window like on the home page but specifically for this pair, in this pool. Expand the window by clicking on the arrow where it shows you the current ATOM:OSMO rate in the pool.

You can see here that a swap of 10 ATOM to OSMO results in less than 0.001% price impact. This means your trade will change the price in the pool by less than 0.001%.

![](https://i.imgur.com/BdzMAqv.png)

Note also that in the image above it says the minimum amount of $OSMO you will receive is 134.22. This means if the prices in the pool change while your trade is being executed and the output amount becomes less than 134.22 OSMO, you will not accept this trade and the transaction will fail. 

This is with the default slippage of 1% set. The expected output is 135.577 OSMO, so multiply that by 99% (1% slippage) and the minimum accepted is 134.22 OSMO.

You can change the slippage settings by clicking on the cog icon on the top right of the swap card. If we change it to 5%, the minimum received before rejecting the trade reduces to 128.77 OSMO. However, the price impact in the pool stays the same.

![](https://i.imgur.com/XdszQb7.png)

Because this pool has such high liquidity - $66 million - even a trade of 1000 ATOM has a very low price impact. The difference in input and output is mostly from the 0.2% swap fee.

![](https://i.imgur.com/qg6xvfd.png)

Now, let's compare with the LINK/OSMO pool, [pool 731](https://app.osmosis.zone/pool/731), which has only $29,500 liquidity. A $150 trade already has 1% impact on the pool prices. 

A $2000 trade creates a 13.8% price impact, and Osmosis warns you of this. It still allows you try to execute the trade with 1% slippage, but it will fail, because only a small percentage of the trade would be able to be filled at 1% slippage.

![](https://i.imgur.com/gGDo9rN.png)

In this case, you would need to either increase the slippage setting to match the price impact on the pool, or make smaller trades to create less impact. Be sure that you are okay with the 'minimum received' amount before executing large trades!

![](https://i.imgur.com/lpOPxVN.png)
