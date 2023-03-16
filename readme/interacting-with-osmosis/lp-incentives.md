Osmosis relies on its users to provide liquidity for trading on the DEX. To encourage this, a percentage of the $OSMO inflation is directed towards incentives for pools. Currently the total inflation that goes towards LP incentives is 13.5%. This can be adjusted with governance proposals such as proposal 364. The current inflation split is as shown below:

![](https://i.imgur.com/xr8o71m.jpg)
 (Current $OSMO Inflation [split](https://hackmd.io/U37CDcTDTC60v1JW-0e4sA?view#Chain-Design))
 
 As well as proposals to adjust this split, there are also regular incentive adjustment proposals, and proposals to incentivise new LP pairs. You can see an example of this in the discussion on Commonwealth about incentivising $FTM [here](https://gov.osmosis.zone/discussion/9921-fantom-incentives).
 
 To account for changes like adding new incentivised pools, there is a semi-automatic incentive adjustment proposal every week. The proposed changes are shown in a spreadsheet linked in the proposal, and then on the live updating [spreadsheet](https://bit.ly/newincentivessheet) as shown below.
 
 ![](https://i.imgur.com/jcbaA9g.png)

You will notice there is also a column on the spreadsheet for 'external APR'. Projects listing their token for trading on Osmosis may choose to incentivise the LPs, which they can do permissionlessly. These are limited time incentives. Let's look at pools 837 and 908 from the spreadsheet excerpt above. 

[Pool 837](https://frontier.osmosis.zone/pool/837) currently has $BLD incentives provided by the Agoric team. It is a set 5000 BLD per day for 14-day unbonding. This means the 5000 BLD is divided between all LP providers who have locked their tokens with 14-day unbonding. If more people lock tokens in the pool, your personal rewards will reduce. Conversely, as people unbond, your rewards will increase.

[Pool 908](https://frontier.osmosis.zone/pool/908) has $BLD as well as $CMDX external incentives. Notice here that the incentives have 21 days remaining. After 21 days it will return to only having swap fees. If you are joining pools based on external incentives, it is good to note how long the incentives run for.

![](https://i.imgur.com/ghvRmdZ.png)

When you unbond from a pool, you will stop receiving rewards, unless it has incentives for lower timeframes. For example, [pool 909](https://frontier.osmosis.zone/pool/909) below has 1-day, 7-day and 14-day unbonding incentives. After unbonding from the 14-day lock, you will receive the 7-day unbonding rate for the first 7 days, and 1-day incentives for the remaining 7 days. After 14 days you will be able to withdraw your liquidity and trade or move your tokens.

Osmosis has recently removed 1-day and 7-day unbonding periods for internal $OSMO incentives in accordance with [proposal 400](https://wallet.keplr.app/chains/osmosis/proposals/400), so now only external incentives are able to have this feature.

![](https://i.imgur.com/QjA8AHb.png)

Liquidity incentives are paid out at epoch each day - roughly 17:15 UTC. You will see your daily rewards added to your [Assets](https://app.osmosis.zone/assets) list after this time. Tokens that have not been officially accepted onto the Osmosis main app will only appear on [Frontier](https://frontier.osmosis.zone/assets). Swap fees do not get paid out but rather add to your LP position.

![](https://i.imgur.com/Pyj6ZfL.jpg)

[Info.osmosis.zone](https://info.osmosis.zone/dashboard) has a handy dashboard to show your daily and accumulated rewards! You can also download a spreadsheet of your rewards history from here.

![](https://i.imgur.com/4ZPwK5O.png)
