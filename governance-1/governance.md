# 🗳 Voting and Proposals

#### **Informal Discussion**

The proposal and voting process begins with informal and high-level proposals on Discord and other channels the community chooses. That would be followed by intermediate proposals with some level of detail on Discourse, which could also be linked to proposed changes outlined in a Pull Request or Issue to the HaloDAO Github.

#### **Formal Proposal and Voting**

Formal proposals and subsequent voting can be kicked off by any HALO token holder who can create a new proposal on [Snapshot](https://snapshot.page/#/) consisting of:

1. The description of the proposal \(potentially with a link to the Github PR or Issue\) 
2. The proposal data itself: an array of multisend transaction payloads executable by the Gnosis Safe module.

Each proposal on Snapshot is linked to a Reality.eth question asking if:

1. The linked Snapshot proposal passed.
2. Did the proposal include the payload, and 
3. Does the payload do what the proposal describes.

If the proposal passes on Snapshot, then Reality.eth should resolve to the same outcome, and after a 24 hour cooldown period, the proposal’s transactions are executable by anyone. Reality will use the HALO ERC20 governance token for the bond. The minimum bond can be set by way of a proposal to the DAO.

#### **Proposal Types**

One thing to note is that various governance proposal types can be categorized into either Self Executing or needing Manual Execution. Self**-**executing proposals are those detailed below that can simply go through the governance process described above and are generally programmable parameters in HaloDAO’s smart contracts. Manual execution, however, would require action from human actors and would not be part of the governance process described above. There would be no “standard way” to handle manually executed proposal types, as it would be something outside the scope of programmable parameters in the smart contracts.

Examples of Self Executing proposal types are the following:

| **Self Executing Proposals** | **Sample value** | **Comment** |
| :--- | :--- | :--- |
| **AMM LP swap fee** | **0.003** | **Equal to 0.3% of the swapped transaction amount** |
| **AMM LP swap fee** | **0.0005** | **Equal to 0.05% of the swapped transaction amount** |
| **Voting cooldown period** | **24 hrs** |  |
| **Voter reward per epoch** | **0.2** | **Equal to 20% of network profits per epoch** |

  


{% hint style="info" %}
To see a more thorough explanation of how governance will work, see the [Litepaper](https://www.halodao.com/litepaper). 
{% endhint %}



