# 🔁 AMM



![](https://lh6.googleusercontent.com/fPoXgsW0GiNhw7sjmSycbArGTPsMrkCvtGi\_1sGrL2jBQAMQvYdansw4A76RoqRMSlb4rcgU0BUIaFJ9hoYqWBoLWUG-UDlnLXFMDQarbfDoFW8IeIqdrJJIExtrClnpDEvLC3wr)

## Overview

The figure above denotes the custom bonding curve that HaloDAO adopts for each liquidity pool in our AMM. When a swap transaction is executed, the corresponding proportion of tokens that remain within the liquidity pool after the swap is reflected on the purple line above.

Swaps can occur in one of two “regions” of the bonding curve:

One region is the “beta” region (points colored in orange), where one token can be exchanged for another at expected real world rates (“FX accurate”). Within this region, traders will be charged a constant fixed fee paid to LPs, just as with any AMM. It is important to note that in the beta region, there is no price slippage and the total amount of assets in the pool obeys a linear relationship – a constant sum invariant behavior.

Outside this “FX accurate” beta region, however, trades will be priced depending on the LP ratio and no longer depending on the real world FX price. Additionally, the swap fees paid to LPs will be dynamic, wherein a trade that moves the token ratio away from “FX rate” or beta region will be charged a higher fee and a trade that moves the token ratio towards “FX rate” or the beta region will be charged a lesser fee. Dynamic swap fees charged outside the beta region, under current configuration, can generate 100x more fees than the constant 5 basis point swap fee within the beta region

The basic takeaway for arbitrageurs is that it is more profitable to balance a stablecoin pool back to the expected token ratios that result in FX accurate swaps, rather than unbalancing the pool in such a way that swaps are not FX accurate. It is also noteworthy that our AMM also consists of halt boundaries that prevent the complete draining of pool liquidity.

## Mechanism&#x20;

When the liquidity composition crosses beyond the beta region, there will be price slippage. As seen from the diagram above, once the composition of tokens crosses point J the graph curves horizontally. In this region we observe that the pool is largely weighted by Token B than Token A. Since the gradient of the slope determines the price of Token A in terms of Token B, this means that the price of Token A decreases between point J to K. Conversely, when the composition of liquidity is largely weighted by Token A than Token B (HI), the graph curves vertically and this means that the price of Token A generally increases between point I to H.

Naturally, this provides an opportunity for arbitrage. Theoretically, given the dynamically increasing trading fees as users trade further away from the beta region coupled with the arbitrage opportunity, users are likely to trade towards the region where there is no price slippage. However to further safeguard our liquidity pools from being completely drained, HaloDAO’s AMM pools have a minimum and maximum allocation parameter which restricts trades from continuing beyond a specific point – Point H and Point K.&#x20;

## Stablecoin Liquidity Pools&#x20;

For our stablecoin AMMs, we are utilising Chainlink price feeds in order to ensure that trades that are executed between the beta region will be traded at FX accurate rates thus mimicking the prices of currencies in traditional financial markets, at least for a certain threshold of the price range.



![](<../../.gitbook/assets/Supported Stablecoins\_14Dec.png>)

​

HaloDAO incentivises liquidity provision and trading between

* asset-backed stablecoins
* synthetic stablecoins
* and important pairings against ETH, WBTC, USDC, USDT and other "must have" cryptocurrencies



{% content-ref url="../../get-started/how-to-swap.md" %}
[how-to-swap.md](../../get-started/how-to-swap.md)
{% endcontent-ref %}



