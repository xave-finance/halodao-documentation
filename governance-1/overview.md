# ⚡️ Governance Model

HaloDAO's voting portal will allow any HALO token holder to stake and vote on proposals initiated by other HALO token holders. Your voting rights are directly proportional to the number of HALO tokens you own.

The HALO token holders can propose and vote for:

* New economic and geographic regions to expand to. 
* New collateral types and synthetics to support across the AMM, and Lending Market.
* Adjust the HALO burn rate. \(to lessen the total HALO supply over time, funded by the Stablecoin Earnings Pools\)
* When to execute buybacks using funds from the Stablecoin Earnings Pools.
* And many other proposal types

#### **Informal Discussion**

![Informal Discussion for Proposal Flow](https://lh3.googleusercontent.com/WywWwla2bJDtETfNJnfllakE_RztlJSpHIpE5TQ8WxukV1xfHKkOhE9nMsYPNsv6CijrpFuyUXOio4QLn0CvhT3xxp6qxUrHJuD5_AXM_rD58Adg-ipL38cbpOy9EnrdX-ndEdgY)

The proposal and voting process begins with informal and high-level proposals on Discord and other channels the community chooses. That would be followed by intermediate proposals with some level of detail on Discourse, which could also be linked to proposed changes outlined in a Pull Request or Issue to the HaloDAO Github.

#### **Formal Proposal and Voting**

![Formal Proposal and Voting Flow](https://lh4.googleusercontent.com/M9GAsB0Md5kxdH0b-VgSyKt5iIYT9RMLug-_WcLOe_nB6vNCyS1JvenxzQIK167EUorx_zZMcrMeotpwPEwqPZGh-D5izAZdnGhO66fgpj8kiaQLeCUYajbwzjBHdf8Avivc99hQ)

Formal proposals and subsequent voting can be kicked off by any HALO token holder who can create a new proposal on [Snapshot](https://snapshot.page/#/) consisting of:

1. The description of the proposal \(potentially with a link to the Github PR or Issue\) 
2. The proposal data itself: an array of multi-send transaction payloads executable by the Gnosis Safe module.

Each proposal on Snapshot is linked to a Reality.eth question asking if:

1. The linked Snapshot proposal passed.
2. Did the proposal include the payload, and 
3. Does the payload do what the proposal describes.

If the proposal passes on Snapshot, then Reality.eth should resolve to the same outcome, and after a 24 hour cooldown period, the proposal’s transactions are executable by anyone. Reality will use the HALO ERC20 governance token for the bond. The minimum bond can be set by way of a proposal to the DAO.







