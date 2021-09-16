# How Vesting Works \(Polygon\)

![](../../.gitbook/assets/screenshot-2021-09-16-at-6.24.00-pm.png)

Polygon users earn Wrapped xRNBW from the farming pools in the same way as Ethereum mainnet users do, with one small difference. Wrapped xRNBW can only be used to claim Wrapped RNBW from the [contract deployed on Ethereum](https://etherscan.io/address/0x47be779de87de6580d0548cde80710a93c502405). The reason for this is that our Rainbow Pool dictates xRNBW:RNBW based on the total supply of the xRNBW token. That combined with our bridge, being a wrapped token bridge, would mint tokens and in turn cause a permanent difference in xRNBW:RNBW price between Polygon and the Ethereum mainnet. 

As a workaround, users may swap their wxRNBW for wRNBW \(or vice versa\) on our [Polygon xRNBW:RNBW pool](https://app.sushi.com/swap?inputCurrency=0xc104e54803aba12f7a171a49ddc333da39f47193&outputCurrency=0x18e7bdb379928a651f093ef1bc328889b33a560c). The price may divert from the true price on Ethereum mainnet, especially after Epoch triggers every 30 days, though we do expect that once an arbitrage opportunity becomes sufficiently profitable, any arbitrageur would take advantage, thus bringing the price back within expected ranges. Of course, there is always the option to redeem xRNBW back on Ethereum mainnet via our bridge. 

{% page-ref page="../../get-started/how-to-earn/how-to-vest-rainbow-pool-polygon-matic/" %}



