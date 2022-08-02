# Lending Market FAQs

## What are hTokens?

hTokens are ERC20, interest bearing tokens, which represents the assets held and accrued fees of HaloDAO's lending protocol. When a user deposits an asset, as a collateral, in a specific reserve, they receive a corresponding amount of hTokens, minted on a 1:1 ratio. The user's hToken balance grows over time as the interest collected is distributed to all hToken holders.

## What are Debt Tokens?

Debt tokens are ERC20, interest accruing tokens, that represents a user's borrow position. When a user opens a borrow position, he can choose between Stable Debt and Variable Debt rates. A user cannot choose stable rate if he borrows the same asset as his collateral.

**Stable Debt Tokens** - rate is fixed for a short period of time but can be rebalanced to respond to market changes.

**Variable Debt Tokens** - rate can increase or decrease depending on the amount of liquidity in the reserve.&#x20;

## What are the Borrow and Earn Rates?

HaloDAO's interest rate model uses a double-slope model that defines the scaling of interest based on the utilization rate on each reserve. Utilization rate is the ratio between the total amount of liquidity vs. the total amount of borrow demand on a reserve. In order to maintain a healthy utilization rate, each reserve has a defined interest rate strategy that can be adjusted based on the following risk parameters:

**Optimal Utilization Rate -** a target range that defines the when the interest rate should scale faster. Interest rate growth is slower if it is below optimal range, otherwise, interest rate growth is faster, if it's above the optimal range. &#x20;

**Interest Rate Slope 1 -** is a constant that represents the scale of interest rate if it is below optimal utilization rate. &#x20;

**Interest Rate Slope 2 -** is a constant that represents the scale of interest rate if it is above optimal utilization rate. &#x20;



## What is Health Factor?

The health factor is the numeric representation of the safety of your deposited assets against the borrowed assets and its underlying value. The higher the value is, the safer the state of your funds are against a liquidation scenario. If the health factor reaches 1, the liquidation of your deposits will be triggered. A Health Factor below 1 can get liquidated.

## How is the price updated?

HaloDAO uses Chainlink for price feeds. Prices are refreshed every time the deviation crosses a certain threshold.
