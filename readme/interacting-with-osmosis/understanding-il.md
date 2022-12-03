# Impermanent Loss

**One of the main considerations for someone adding assets to traditional liquidity pools is the risk of impermanent loss. **_**Don't be fooled by the strange name - the effect can be very permanent.**_

**Impermanent loss is an effect of token prices changing in a liquidity pool.**

If you are \[\[staking]] your OSMO coins, you will always retain that number of OSMO, and the value of your holdings fluctuates only based on the price of OSMO. However when you pair it with another token in a \[\[liquidity pool]], you are likely to exit the pool with a different number of OSMO than you started with. Sometimes it turns out that you would have been better off just holding your coins instead of providing liquidity. This opportunity cost is called impermanent loss.

<img src="https://image.scribehow-prod.com/Mfh-W8wB33T1ae-w4_lPz-Sk50xu8MrR-MRdQATBKTU/zoom:1.5013404825737264/enlarge:true/crop:746:420:nowe:650:361/wm:0:nowe:535:96:0.08928571428571429/aHR0cHM6Ly9jb2xvbnktcmVjb3JkZXIuczMuYW1hem9uYXdzLmNvbS9maWxlcy8yMDIyLTExLTI1L2Y5ZmNiYjdlLWMxZjUtNGRhZi04YjYzLTg4OTZlZGUyNmEyYi91c2VyX2Nyb3BwZWRfc2NyZWVuc2hvdC5qcGVn" alt="" data-size="original">\
**To understand how and why IL happens, it will help to learn some basic mechanics behind liquidity pools, and the concept of arbitrage.**

In an established liquidity pool, the price of the tokens there is affected only by buy/sell pressure on that pool. Since the pool doesn't know or care what the market is doing, traders can now take advantage of price differences between this and other platforms by arbitrage trading.\
Consider this scenario-- You have some OSMO and BNB in a pool. Suddenly, the market price of BNB drops sharply. Traders can still come and sell their BNB to this pool at the original (higher) price, and take more of your OSMO out.

The more BNB sold into the pool, the lower the price for that asset will drop. This typically continues until the price of the tokens in that pool nears average market price, and there is no longer a financial incentive to continue.

With these swaps of BNB into the pool, your LP-token will now consist of more BNB and less OSMO, and the value of your holdings is lower because of the price decline on BNB.

![](https://image.scribehow-prod.com/C5lDoRqoXKxS9URfb0coRyzmmTdPhi\_FuG5doo0qIaU/zoom:1.5013404825737264/enlarge:true/crop:746:420:nowe:436:330/wm:0:nowe:535:289:0.08928571428571429/aHR0cHM6Ly9jb2xvbnktcmVjb3JkZXIuczMuYW1hem9uYXdzLmNvbS9maWxlcy8yMDIyLTExLTI1LzU0OWQ1NzU3LTQ3ZTctNGJiOC05NTU1LWExNGVkN2Y4ZjFmYy9zY3JlZW5zaG90LnBuZw)

**The more dramatic the price change, the more loss there is. If you have a pair of tokens that generally move together (eg OSMO and stOSMO), the risk of impermanent loss is reduced. Stablecoin pairs are also popular, though not immune to IL. You can use a calculator like https://dailydefi.org/tools/impermanent-loss-calculator/ for estimating potential IL on your chosen pair.**\
The reason the term is called 'impermanent' loss is because the fluctuation in a price like the example above can be a short-term anomaly. If you don't remove your liquidity at that moment in time, the loss has not been made permanent. The price of the token (in this case BNB) may return to its previous level and then your LP token is more or less back to where it was.

If you do remove your liquidity when these extreme price movements happen, you make the 'impermanent' loss permanent, since adding/removing liquidity is at a fixed ratio.

![](https://image.scribehow-prod.com/UKVy5y6-cCrclfzH97YoCtkdsWSlAr5Y\_nGNMelKbCc/zoom:1.5013404825737264/enlarge:true/crop:746:420:nowe:8:344/wm:0:nowe:535:418:0.08928571428571429/aHR0cHM6Ly9jb2xvbnktcmVjb3JkZXIuczMuYW1hem9uYXdzLmNvbS9maWxlcy8yMDIyLTExLTI1LzkyZGVkMGFkLTQ5MzQtNGJjMC1hZTNmLTkwZTc3MjhhYTQxOC9zY3JlZW5zaG90LmpwZWc)\
**After reading this you may wonder why people take the risk in providing liquidity. DEXes need to provide an incentive for users to provide liquidity: earning the fees on swaps into the pool often isn't attractive enough on its own.**

In Osmosis' case, a portion of $OSMO's annual inflation is reserved for this purpose. Osmosis has governance proposals for stakers to vote on which pools get incentivised. New coins and tokens that come to Osmosis regularly provide incentives of their own token, as well.

These incentives attract liquidity providers and double as a hedge against impermanent loss.

![](https://image.scribehow-prod.com/4yTjdxCJhL1HlUUjike36stM6Uf4VR\_J9plc4Igeh3E/zoom:1.5013404825737264/enlarge:true/crop:746:420:nowe:586:330/wm:0:nowe:535:289:0.08928571428571429/aHR0cHM6Ly9jb2xvbnktcmVjb3JkZXIuczMuYW1hem9uYXdzLmNvbS9maWxlcy8yMDIyLTExLTI1L2FjMGQwMTVmLTYxYTQtNGMyZS1iZjIwLTUyNzdkOTgxZGYzZi9zY3JlZW5zaG90LnBuZw)\
**Whether prices increase or decrease, there is still the risk of impermanent loss. As you can see in this chart, the loss is much more significant if one of the tokens does a 4x compared to a 1x.**

![](https://image.scribehow-prod.com/eAPA4Qw\_a6aJ7YdeqcweHsafgMT4PFWEK0PXLwFFN28/zoom:1.5013404825737264/enlarge:true/crop:746:420:nowe:426:240/wm:0:nowe:535:289:0.08928571428571429/aHR0cHM6Ly9jb2xvbnktcmVjb3JkZXIuczMuYW1hem9uYXdzLmNvbS9maWxlcy8yMDIyLTExLTI1L2RhMjdmMmQxLWU4ZDktNGVhMC1iZDJlLThlOGZiOGUyYzlkMC9zY3JlZW5zaG90LnBuZw)\
**Considering the above points may help guide you with your choices of liquidity pairs. Providing liquidity often yields higher APRs than staking, which can be worth it as long as you know what you're getting into!**

![](https://image.scribehow-prod.com/k8RljORdVz28sDJVdCbx\_hcp0h7-hAJ-y8q6Ib5qkIo/zoom:2.007168458781362/enlarge:true/crop:558:420:nowe:0:8/wm:0:nowe:533:395:0.08928571428571429/aHR0cHM6Ly9jb2xvbnktcmVjb3JkZXIuczMuYW1hem9uYXdzLmNvbS9maWxlcy8yMDIyLTExLTI1LzJkY2QxYzk4LTkyMzUtNDc1YS1hOTA2LTA4M2Y4MGNiY2IzMS9zY3JlZW5zaG90LnBuZw)
