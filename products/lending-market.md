# 🏦 Lending Market

## Overview&#x20;

Our Lending Market allows users to deposit first ETH, WBTC and popular USD pegged stablecoins as collateral to borrow various local currency pegged stablecoins, in contrast to most lending protocols in the DeFi space that give no focus to regional currencies.&#x20;

![](<../.gitbook/assets/Money Market-2.png>)

## Mechanism

Lenders who supply their tokens to our lending market will receive interest yield according to the current supply APR. The supply tokens are then sent to the protocol and become available for other users to borrow. The smart contract then issues H-tokens that represent a claim on those deposited supply tokens and the interest yielded over time. For example, lenders that supply 1 USDC will receive 1 hUSDC and over time, that 1 hUSDC will be worth more than 1 USDC.&#x20;

Over-collateralization is used to ensure that all positions remain backed. This means that the users who want to borrow funds have to supply tokens in a form of collateral that is worth more than the actual loan that they want to take.

## What is the limit of the amount I can borrow?&#x20;

The amount that can be borrowed is dependent on 2 factors:\
\
1\. Amount of supplied tokens in the pool\
2\. Maximum Loan-to-Value (LTV) ratio.

For point 1, it is unlikely to be a huge problem unless the borrower wants to borrow a large sum. As for point 2, the Maximum Loan-to-Value ratio represents the maximum borrowing power of a specific collateral. For example, if a collateral has a LTV of 75%, the user can borrow up to 0.75 worth of ETH in the principal currency for every 1 ETH worth of collateral.

## What happens when the value of the collateral drops?&#x20;

When the value of the collateral falls below the liquidation threshold, the user will have the collateral liquidated as the borrow position will now be considered undercollateralized. For example, if a collateral has a liquidation threshold of 80%, it means that the loan will be liquidated when the debt value is worth 80% of the collateral value.

When liquidation occurs, liquidators repay part or all of the outstanding borrowed amount on behalf of the borrower. In return, they can buy the collateral at a discount and keep the difference as a bonus!

{% hint style="info" %}
Lending market will be included in the v1 launch. See [roadmap](../roadmap/overview.md).
{% endhint %}

\
