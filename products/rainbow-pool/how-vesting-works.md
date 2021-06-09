# How Vesting Works

1. When a user stakes their LP tokens on the [Farm page](https://app.halodao.com), they will be rewarded with RNBW tokens proportionate to their LP tokens. 
2. Their RNBW tokens are automatically deposited into the Rainbow contract and the user will receive the proportionate amount of xRNBW in return.
3. Over time, xRNBW will be worth more and more RNBW tokens due to 20% of monthly RNBW liquidity rewards being deposited into the Rainbow Pool. 

![](../../.gitbook/assets/protocol-overview%20%281%29.png)

The following is a walkthrough on how holding xRNBW yields more RNBW over time. Let’s make the following assumptions using the classic Alice and Bob example:

1. 1 epoch is 1 day \(in real life it will be 1 month\)
2. RNBW Vesting Reward is equal to 1 RNBW
3. RNBW Vesting Reward is paid out per epoch
4. Alice earns 1 RNBW in 1 epoch for supplying liquidity to HaloDAO
5. Alice is the first liquidity provider of the protocol during epoch 1
6. In epoch 2, Bob then provides liquidity after Alice and also earns 1 RNBW in epoch 2

| Event | Epoch | Action | xRNBW:RNBW price | xRNBW:RNBW total supply |
| :--- | :--- | :--- | :--- | :--- |
| Alice earns 1 RNBW | 1 | 1 RNBW auto deposited to Rainbow contract |  |  |
| Alice receives 1 xRNBW | 1 | Rainbow contract mints 1 xRNBW and locks 1 RNBW | 1 xRNBW = 1 RNBW | 1 xRNBW, 1 RNBW |
| 1 RNBW vesting reward sent to Rainbow contract by protocol | 1 | No xRNBW is minted, which increases the price of xRNBW relative to RNBW | 1 xRNBW = 2 RNBW | 1 xRNBW, 2 RNBW |
| Bob earns 1 RNBW | 2 | 1 RNBW auto deposited to Rainbow contract |  |  |
| Bob receives 0.5 xRNBW | 2 | Rainbow contract mints 0.5 xRNBW and locks 1 RNBW | 1 xRNBW = 2 RNBW | 1.5 xRNBW, 3 RNBW |
| 1 RNBW vesting reward sent to Rainbow contract by protocol | 2 | No xRNBW is minted, which increases the price of xRNBW relative to RNBW | 1 xRNBW = ~2.67 RNBW | 1.5 xRNBW, 4 RNBW |
| Alice claims RNBW using 1 xRNBW | 2 | 1 xRNBW is burned, 2 RNBW is withdrawn from Rainbow contract | 1 xRNBW = ~2.66 RNBW | 0.5 xRNBW, 1.33 RNBW |
| Bob claims RNBW using 0.5 xRNBW | 2 | 0.5 xRNBW is burned, 1.33 RNBW is withdrawn from Rainbow contract | 0 xRNBW = 0 RNBW | 0 xRNBW, 0 RNBW |
| Alice earns 1 RNBW | 3 | 1 RNBW auto deposited to Rainbow contract |  |  |
| Alice receives 1 xRNBW | 3 | Rainbow contract mints 1 xRNBW and locks 1 RNBW | 1 xRNBW = 1 RNBW | 1 xRNBW, 1 RNBW |

Over time as RNBW vesting rewards are deposited into the Rainbow vesting contract the price of xRNBW in terms of RNBW will increase. Of course, 1 epoch will not just be 1 day but 1 month in actual operations, and Alice and Bob in this example won’t necessarily claim all RNBW and burn total xRNBW supply \(thus resetting xRNBW:RNBW price\) at the same time,  but this serves as a simple simulation of the vesting mechanism. If you think this sounds familiar, that is because we forked the Rainbow contract from Sushi’s SushiBar but made some slight changes, namely;

1. Instead of a ⅔ vesting schedule, the liquidity provider will automatically earn RNBW rewards from the Rainbow contract and give the liquidity provider xRNBW. We figured this approach would save the user gas, automatically vest the user to earn more RNBW \(as long as you stick around for at least a month interval\) but still allow the flexibility of real-time withdrawal at any time.
2. In addition to depositing network profits \(exact amount and time interval to be determined after HaloDAO profit drivers are enabled at AMM and Lending Market launch\), 20% of monthly RNBW liquidity rewards over 5 years will be sent to the Rainbow vesting contract every month. This increases xRNBW APY and further incentivises long-term holding.

