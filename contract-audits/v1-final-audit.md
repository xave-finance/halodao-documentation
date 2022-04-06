---
description: >-
  Attached are the audit reports for v1 with all issues marked as "Closed"
  (meaning the auditors have verified that changes have addressed the previously
  "Open" issues).
---

# v1 Final Audit

## **Pot of Gold**

* There were 2 issues (1 minor and 1 medium) pointed out during the audit review. These issues have  been resolved as of commit hash`70f96fc88795a1ebfe0ab24540ba2f472a59c7ec`
* The repository used by the auditors, Monoceros Alpha, is also now publicly accessible here**:** [https://github.com/HaloDAO/review-halo-rewards-2021-08](https://github.com/HaloDAO/review-halo-rewards-2021-08)

{% file src="../.gitbook/assets/PotOfGold Audit.pdf" %}
Pot of Gold Audit
{% endfile %}

## **AMM**

* Minor changes were attempted on the original forked code, however our auditors recommended that we stick with the original code which has been audited previously as seen from the attachment below.

{% file src="../.gitbook/assets/2021-05-03-Trail_of_Bits.pdf" %}
Trail of Bits
{% endfile %}

## **AMM v1 Audit 2**

* There were some minor recommendations which generally involved the removal of bespoke codes that are not used in HaloDAO’s AMM. The initial review focused on the HaloDAO AMM repository, identified by the commit hash `aeb29effd3d379b1ffdae6bf82b39bfae262a6c4` . A further code change was merged into the repository from commit hash `c22d26a49a44ad6409190572da384cb724435201`
* The repository used by the auditors, Monoceros Alpha, is also now publicly accessible here: [https://github.com/HaloDAO/amm-v1](https://github.com/HaloDAO/amm-v1)

{% file src="../.gitbook/assets/AMM v1 Audit 2 (1).pdf" %}

## **Bridge Smart Contracts**

* This Bridge Contract Audit covers the smart contract components of our wrapped token bridge
* There were some minor recommendations, which have been addressed at commit hash `7fab901ff5aa136972ce2533f39f8d912e5e363c`
* The repository used by the auditors, Monoceros Alpha, is also now publicly accessible here**:** [https://github.com/HaloDAO/review-halo-token-bridge-2021-08](https://github.com/HaloDAO/review-halo-token-bridge-2021-08)

{% file src="../.gitbook/assets/Bridge Contracts Audit (1).pdf" %}
Bridge Contract Audits
{% endfile %}

## **Bridge Handler**

* This Bridge Handler Audit covers the portion of the bridge that essentially listens for emitted events on the source chain and triggers corresponding actions on the destination chain and vice versa (a wrapped token bridge)
* There were 2 major issues found, regarding the number of block confirmations required to consider a transaction finalized on each chain. These have been addressed at commit hash `2c54d69a75fddaabc97eb140509c112ec8575828`
* The repository used by the auditors, Monoceros Alpha, is also now publicly accessible here**:** [https://github.com/HaloDAO/review-halo-bridge-handler-2021-08](https://github.com/HaloDAO/review-halo-bridge-handler-2021-08)

{% file src="../.gitbook/assets/Bridge Handler Audit (1).pdf" %}
Bridge Handler Audit
{% endfile %}

## **Lending Market**

* This Lending Market Audit covers the smart contract components of our lending market.
* There were some minor recommendations and 1 medium issue found. The recommendations were not security issues but are general improvements that will bring value to the developers and the community reviewing and using the product. These have been addressed at commit hash `01486a398b0aa36b9798ba06fce11b5d3376909d`
* The repository used by the auditors, Monoceros Alpha, is also now publicly accessible here: [https://github.com/akiratechhq/review-halo-dao-lending-market-2021-10](https://github.com/akiratechhq/review-halo-dao-lending-market-2021-10)

{% file src="../.gitbook/assets/Lending Market v1.pdf" %}

