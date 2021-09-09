---
description: >-
  Attached are the audit reports for v1 with all issues marked as "Closed"
  (meaning the auditors have verified that changes have addressed the previously
  "Open" issues).
---

# v1 Final Audit

## **Pot of Gold**

* There were 2 issues \(1 minor and 1 medium\) pointed out during the audit review. These issues have  been resolved as of commit hash`70f96fc88795a1ebfe0ab24540ba2f472a59c7ec`
* The repository used by the auditors, Monoceros Alpha, is also now publicly accessible here**:** [https://github.com/HaloDAO/review-halo-rewards-2021-08](https://github.com/HaloDAO/review-halo-rewards-2021-08)

{% file src="../.gitbook/assets/potofgold-audit.pdf" caption="Pot of Gold Audit" %}

## **AMM**

* Minor changes were attempted on the original forked code, however our auditors recommended that we stick with the original code which has been audited previously as seen from the attachment below.

{% file src="../.gitbook/assets/2021-05-03-trail\_of\_bits.pdf" caption="Trail of Bits" %}

## **Bridge Smart Contracts**

* This Bridge Contract Audit covers the smart contract components of our wrapped token bridge
* There were some minor recommendations, which have been addressed at commit hash `7fab901ff5aa136972ce2533f39f8d912e5e363c`
* The repository used by the auditors, Monoceros Alpha, is also now publicly accessible here**:** [https://github.com/HaloDAO/review-halo-token-bridge-2021-08](https://github.com/HaloDAO/review-halo-token-bridge-2021-08)

{% file src="../.gitbook/assets/bridge-contracts-audit \(1\).pdf" caption="Bridge Contract Audits" %}

## **Bridge Handler**

* This Bridge Handler Audit covers the portion of the bridge that essentially listens for emitted events on the source chain and triggers corresponding actions on the destination chain and vice versa \(a wrapped token bridge\)
* There were 2 major issues found, regarding the number of block confirmations required to consider a transaction finalized on each chain. These have been addressed at commit hash `2c54d69a75fddaabc97eb140509c112ec8575828`
* The repository used by the auditors, Monoceros Alpha, is also now publicly accessible here**:** [https://github.com/HaloDAO/review-halo-bridge-handler-2021-08](https://github.com/HaloDAO/review-halo-bridge-handler-2021-08)

{% file src="../.gitbook/assets/bridge-handler-audit \(1\).pdf" caption="Bridge Handler Audit" %}

