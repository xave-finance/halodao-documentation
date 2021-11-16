# Overview

![](<../.gitbook/assets/Environments Overview.png>)

HaloDAO maintains two copies of the protocol on the Ethereum mainnet.&#x20;

1. The Beta App, also called "LolliDAO", where we deploy _bleeding edge, unaudited_ code that cannot be tested for economic behaviors on a testnet like Kovan or Ropsten. &#x20;
2. The Production App, our main "HaloDAO", once the code has gone through some kind of limited battle testing.&#x20;

Testnets are great for integration and unit testing, however it cannot replicate an environment with real monetary motivations. In our development flow, we first test that new features or products work as they should on a testnet, then we test economic behaviors at a smaller scale, conduct security audits and bug bounties on Beta, then we finally deploy to Production

##
