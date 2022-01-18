# Polygon Matic

## **Halonauts send tokens from Chain A to Chain B**

![](<../../.gitbook/assets/Bridge\_SendsAtoB (1).png>)

The HaloDAO Bridge sits between the ETH Mainnet and other EVM Compatible chains - Polygon being the first Layer 2 chain targeted for implementation.

When a Halonaut deposits tokens using the bridge from Chain A to Chain B, the deposit event will trigger the Primary Bridge Smart contract where the Event Broker Service will call upon the HaloDAO Bridge Handler Endpoint. The Bridge Handler script calls the `mint` function on the Secondary bridge Smart Contract to create the respective wrapped tokens on the destination chain (Chain B).

For example, when a Halonaut deposits TCAD into our Bridge from ETH Mainnet to Polygon Matic chain, user will receive Wrapped TCAD (wTCAD) on their ERC-20 wallet on the Polygon (Matic) Network where they can now choose to swap or supply liquidity to our liquidity Pools!

## **Halonauts Redeem tokens from Chain B to Chain A**

![](<../../.gitbook/assets/Bridge\_RedeemsBtoA (1).png>)

When a Halonaut intends to redeem their tokens from Chain B to Chain A, the mechanics mentioned above are generally replicated. First, the deposit event will trigger the Primary Bridge Smart contract where the Event Broker Service will call upon the HaloDAO Bridge Handler Endpoint. The Bridge Handler script calls the burn function on the Secondary bridge Smart Contract to burn the existing wrapped token on Chain B and at the same time releasing the original deposited tokens to the user **** Chain A.

For example, when the Halonaut intends to redeem TCAD from Polygon to Matic chain, the user will deposit the Wrapped TCAD into our bridge and execute the transaction. By doing so, the wrapped TCAD will be burnt on the Polygon Chain and a proportional amount of TCAD will be released on the ETH Mainnet.\
****\
****





