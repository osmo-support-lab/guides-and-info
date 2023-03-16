Sometimes it is not possible to IBC transfer assets using d'apps. In these cases you can manually IBC transfer between blockchains using the Keplr wallet browser extension. Before you attempt this, please take note of the following:

🚨 Tokens can only be sent by IBC either to or from their home network. That means if you want to send $ATOM from Osmosis to Evmos, it must first be transferred from Osmosis back to its home blockchain, Cosmos, before being transferred on to Evmos. If you IBC-transfer $ATOM directly from Osmosis to Evmos, it will be an unusable token when it arrives on Evmos.

🚨 Never IBC transfer assets to a CEX or anywhere else that requires a memo! IBC transfers do not retain the memo across chains.‍

1. Begin by enabling Developer Mode in Keplr's Settings. Keplr will now display an IBC Transfer button below the tokens in each wallet.

![](https://i.imgur.com/7cxUp8R.png)

![](https://i.imgur.com/kSeiKxQ.png)

2. In this example, we will be transferring $EVMOS from Osmosis back to its native blockchain, Evmos. Have your Evmos wallet address handy.

Notice that the $EVMOS in Osmosis shows 'Evmos channel-204'. We will use this in the next step.

Press the button at the bottom of Keplr to begin the IBC transfer.

![](https://i.imgur.com/aVyygAR.png)

3. Click to add a new IBC transfer channel.

![](https://i.imgur.com/DOSQBql.png)

4. As the $EVMOS in Osmosis is on channel-204, as we noted before, we will add channel-204 as the channel here. It needs to be written as **channel-204**, not just 204, to be accepted.

![](https://i.imgur.com/wtt1qWs.png)

5. If you are sending a token from its native blockchain to another chain, you will need to find the channel another way. You can use [mintscan.io](https://mintscan.io/) to assist with this. Consider checking with the projects' Telegram or Discord communities if you are not sure.

In the screen below, you can see the channels between Osmosis and Evmos are channel-204 and channel-0. 204 is the channel we are using, to transfer **from Osmosis to Evmos.** Channel-0 is the channel for sending **from Evmos to Osmosis.**

![](https://i.imgur.com/MCp1lWN.png)

6. Some blockchains have multiple relayer channels to one chain, as can be seen with Stargaze below. Here you would choose the channel that has the most activity - in Stargaze's case channel-75 (from Osmosis to Stargaze) or channel-0 (from Stargaze to Osmosis). 

Again, if you are unsure, and have no other option but to use a manual IBC transfer, check with an admin in an official community channel. It is also a good idea to do a test transfer before sending the full amount.

![](https://i.imgur.com/7OQcafW.png)

7. Once you have the channel saved, you can continue by pasting your Evmos address in the Recipient field.

![](https://i.imgur.com/CzLYTkE.png)

8. Enter the amount you wish to transfer, and finalise the transaction.

![](https://i.imgur.com/5hM7tFV.png)

9. Once you have submitted the transaction, it can take a few minutes to reach the destination. Your balance will be updated in Keplr once it arrives. In other d'apps, you may need to refresh the page to see your new balance.

![](https://i.imgur.com/aMskYuu.png)

🧪 Tip! It is wise to first check if relay channels are clear, especially if you are transferring to/from a less known blockchain. Info.osmosis.zone/ibc shows the backlog of transactions to/from Osmosis, indicating which channels are congested/blocked and should not be used at that time. When there is a significant number of pending transactions, there is an underlying issue which will need to be addressed by that protocol's team.

![](https://i.imgur.com/di8ncc4.png)

* For IBC transfers that do not involve Osmosis, you can use mintscan.io to check pending transactions.

![](https://i.imgur.com/2QzQRgz.png)
