# How to Deposit Tokens using the Bridge

![](../../.gitbook/assets/bridge-ethereum-to-poly.gif)

1. Click this link [https://app.halodao.com/#/bridge](https://app.halodao.com/#/bridge) to go to the Bridge page
2. On the “from” network box the Ethereum mainnet is selected (Selecting otherr networks will trigger a withdrawal process)
3. Click the “to” network box to select the destination network (Networks supported are Ethereum Mainnet and Polygon)
4. Click the asset dropdown to select the asset that you want to bridge
5. Enter the amount
6. Click “Approve”
7. Click “Next” 
8. Confirmation modal with details will pop up, click “Confirm.”
9. Once the transaction confirms, you should be able to receive the wrapped tokens on the selected “to” network.  

**Fees: **Bridging from ETH to MATIC costs 1 unit of token Bridging from MATIC to ETH costs 20 unit of tokens

_Note for both deposit and withdraw: For added security, the bridge waits for a transaction finality before it will update your balance on the selected destination network. This may take a few minutes depending on the source network selected. _

1. _If the source network is Ethereum mainnet, it will wait for 20 block confirmations (about 5 minutes) before balance gets updated on the destination network._
2. _If the source network is Polygon mainnet, it will wait for 192 block confirmations (about 6 to 7 minutes) before balance gets updated on the destination network._
