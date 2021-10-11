# 🥂 Proposal Types

One thing to note is that various governance proposal types can be categorized into either **self-executing** or needing **manual execution**. Self**-**executing proposals are those detailed below that can simply go through the governance process described above and are generally programmable parameters in HaloDAO’s smart contracts. Manual execution, however, would require action from human actors and would not be part of the governance process described above. There would be no “standard way” to handle manually executed proposal types, as it would be something outside the scope of programmable parameters in the smart contracts.

Examples of self-executing proposal types are the following:

| **Self Executing Proposals** | **Sample value** | **Comment**                                      |
| ---------------------------- | ---------------- | ------------------------------------------------ |
| AMM LP swap fee              | 0.003            | Equal to 0.3% of the swapped transaction amount  |
| AMM LP swap fee              | 0.0005           | Equal to 0.05% of the swapped transaction amount |
| Voting cooldown period       | 24 hrs           |                                                  |
| Voter reward per epoch       | 0.2              | Equal to 20% of network profits per epoch        |

{% hint style="info" %}
Refer to the [governance roadmap](../roadmap/governance-roadmap.md) for the approx. schedule of version releases.
{% endhint %}
