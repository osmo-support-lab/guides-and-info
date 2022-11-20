# BRIDGING-AXELAR

# Bridging with Axelar


The Axelar bridge has been chosen as the canonical bridge between Osmosis and EVM blockchains. It is great for bringing in tokens from outside of the Cosmos. This process requires both Keplr and Metamask wallets. In this example we will be bridging USDC from Avalanche to Osmosis.**

The Axelar bridge accepts native USDC on Ethereum, or "pre-wrapped" Axelar USDC on other chains.  If you have USDC on Avalanche, Fantom or Polygon, you can swap to axlUSDC on curve.fi, as shown in this Avalanche example.

🔗 Avalanche: Swap USDC.e to axlUSDC: https://avax.curve.fi/factory/59

🔗 Polygon: Swap USDC to axlUSDC: https://polygon.curve.fi/factory/221

🔗 Fantom: Swap USDC to axlUSDC: https://ftm.curve.fi/factory/85

![](https://image.scribehow-prod.com/KoRaSPpMBRVtdp5APSe46UQFJpCG8LmF9CsiczjtL3I/zoom:1.5013404825737264/enlarge:true/crop:746:420:nowe:376:265/wm:0:nowe:535:289:0.08928571428571429/aHR0cHM6Ly9jb2xvbnktcmVjb3JkZXIuczMuYW1hem9uYXdzLmNvbS9maWxlcy8yMDIyLTEwLTE4LzQzOWUwZjcyLTRmMjMtNGZjMC04MjViLTY1YTQzNzBlZjBjZi9GaWxlLnBuZw)

**2. Once you have axlUSDC, or another token that can be bridged and used on Osmosis, connect to the Axelar bridge at satellite.money with both your Keplr and Metamask wallets.**

![](https://image.scribehow-prod.com/-gQT05jPt0Gc6qG--s0LsFQaYDJ97YxQ6oOn7H-JZ2I/zoom:1.5013404825737264/enlarge:true/crop:746:420:nowe:376:265/wm:0:nowe:535:289:0.08928571428571429/aHR0cHM6Ly9jb2xvbnktcmVjb3JkZXIuczMuYW1hem9uYXdzLmNvbS9maWxlcy8yMDIyLTEwLTE4Lzk2ZmM1MWNlLTkzMWEtNDM4Mi05ODJlLTllNjc3NjViMDBjMy9GaWxlLmpwZWc)

**3. Choose your origin, destination chain, and token. You can then auto-fill the destination address from Keplr or paste a different address if the destination is not your connected wallet. The relayer fee and estimated wait time depends on the chain you are bridging to/from. You will also need the chain's native coin for gas, in this case AVAX.**

![](https://image.scribehow-prod.com/FqX_R8S-fsJp7bZLDGz0xvCpXmg2WykstSJ9NenxWLQ/zoom:1.5013404825737264/enlarge:true/crop:746:420:nowe:376:265/wm:0:nowe:535:289:0.08928571428571429/aHR0cHM6Ly9jb2xvbnktcmVjb3JkZXIuczMuYW1hem9uYXdzLmNvbS9maWxlcy8yMDIyLTEwLTE4LzZiNjhhOTkxLTEwNzAtNGNlYi04YjZjLTA1YTc3NWJlM2U3MC9GaWxlLmpwZWc)

**4. Click to generate a one-time bridge deposit address.**

![](https://image.scribehow-prod.com/7ZMDn7lRx_b_QIa24AEOrQdTMSheTbaqMsQpodg_Z3c/zoom:1.5013404825737264/enlarge:true/crop:746:420:nowe:376:265/wm:0:nowe:535:289:0.08928571428571429/aHR0cHM6Ly9jb2xvbnktcmVjb3JkZXIuczMuYW1hem9uYXdzLmNvbS9maWxlcy8yMDIyLTEwLTE4LzhlYTVmODM2LTVlMTItNGU3Yy04MzdmLWM5YWFlOGFjOWZiOC9GaWxlLnBuZw)

**5. Check that you understand the warning message and confirm.**

![](https://image.scribehow-prod.com/TJ2L08qYyuUz-16Rc3P0eh_TD_vsFO2PEVOyWNb0lFQ/zoom:1.5013404825737264/enlarge:true/crop:746:420:nowe:376:265/wm:0:nowe:535:289:0.08928571428571429/aHR0cHM6Ly9jb2xvbnktcmVjb3JkZXIuczMuYW1hem9uYXdzLmNvbS9maWxlcy8yMDIyLTEwLTE4LzI5Yzk5MmFkLTc5YTktNGUyZC05NDc4LTU1MGE3Y2VhNzNiZi9GaWxlLnBuZw)

**6. Click on the icon to deposit to the temporary deposit address directly from Metamask.**

![](https://image.scribehow-prod.com/KLJAs0Bx17iDWa9JaArP8wr7tK7Gb-8g0GEmv7i7dV4/zoom:1.5013404825737264/enlarge:true/crop:746:420:nowe:376:265/wm:0:nowe:535:289:0.08928571428571429/aHR0cHM6Ly9jb2xvbnktcmVjb3JkZXIuczMuYW1hem9uYXdzLmNvbS9maWxlcy8yMDIyLTEwLTE4L2NlYWFkY2VkLTY3MDctNDIzNi1iYTM4LWI0ZDQ1M2FiYjdkNC9GaWxlLnBuZw)

Tip - If you want to send USDC from a centralised exchange to Osmosis, you can withdraw from the CEX directly to a temporary bridge address instead of depositing with Metamask. Make sure to withdraw on the ETH network and have Ethereum selected on the Axelar bridge.**

**7. Choose the amount you wish to bridge and press send.**

![](https://image.scribehow-prod.com/7QQQHZgaW77Pr3JPgaekVmP8NcsFAkuxddbOJk5mROE/zoom:1.5013404825737264/enlarge:true/crop:746:420:nowe:376:265/wm:0:nowe:535:289:0.08928571428571429/aHR0cHM6Ly9jb2xvbnktcmVjb3JkZXIuczMuYW1hem9uYXdzLmNvbS9maWxlcy8yMDIyLTEwLTE4L2M1NTM4NTI1LTZkNWQtNDZhMC1iMTA5LTY3MWU5OGE3ODIzOS9GaWxlLnBuZw)

**8. Check that everything looks right in the Metamask pop-up and confirm your transaction. The bridge page will then show you the confirmations before it is complete.**

![](https://image.scribehow-prod.com/psA6QhtCpGR8m8nQqc_yh6b-qRuFy7IOQ-7MVQdcRVQ/zoom:1.5013404825737264/enlarge:true/crop:746:420:nowe:376:265/wm:0:nowe:535:289:0.08928571428571429/aHR0cHM6Ly9jb2xvbnktcmVjb3JkZXIuczMuYW1hem9uYXdzLmNvbS9maWxlcy8yMDIyLTEwLTE4LzdjZmJhNDRiLTM5ZGUtNDBkNC04NWFkLTI0ODgxYzM5MTZmNS9GaWxlLmpwZWc)

**9. Success! Your funds have been transferred to Osmosis. You should see the balance in your Keplr wallet browser extension and on the Assets page of Osmosis. To see the transaction details, look up your Osmosis wallet address on the block explorer mintscan.io.**

![](https://image.scribehow-prod.com/Mpb8ZgkfuGVfmlqTj8k8-6RUSYR40Yl16AGb-xLxp1w/zoom:1.5013404825737264/enlarge:true/crop:746:420:nowe:376:265/wm:0:nowe:535:289:0.08928571428571429/aHR0cHM6Ly9jb2xvbnktcmVjb3JkZXIuczMuYW1hem9uYXdzLmNvbS9maWxlcy8yMDIyLTEwLTE4LzI3MTY1YTFhLTRmMDYtNDY1ZS1iY2FjLTMzNmJjZGM5NjI3Ny9GaWxlLnBuZw)



