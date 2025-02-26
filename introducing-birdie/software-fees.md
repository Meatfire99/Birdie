# Software Fees

Birdie is a blockchain software service that seamlessly connects various DeFi protocols, enabling users to supply tokens and automate yield farming.

The fees incurred when using Birdie primarily include:

* Transaction Gas Fees: These are network fees associated with executing blockchain transactions, independent of Birdie.
* Underlying Protocol Fees: When interacting with the underlying protocols for yield farming, fees are charged as per their established guidelines.
* Automated Farming and Harvesting Costs: To facilitate automated yield farming, harvesting, and reinvestment, additional transaction fees are incurred. To cover the costs of operating the software, a predetermined amount of ETH is charged for each such transaction.

To prevent excessive transaction fees, a minimum threshold is set for the automated harvest transactions. If the yield accumulated in a pool does not exceed this threshold, the transaction is deferred to the next cycle. The threshold is typically set at ten times the transaction fee.

For instance, if the transaction fee is 0.0001 ETH, the threshold would be 0.001 ETH. Before initiating an automated harvest, the pool’s yield is checked to ensure it exceeds 0.001 ETH. If not, no transaction occurs, and the process will be reattempted in the next cycle.

Notably, the set transaction fee is not imposed on an individual basis but is apportioned among all participants in the pool based on their share of the supplied assets. Therefore, an individual user’s fee is significantly lower than the set fee. For example, in a pool with a transaction fee of 0.0001 ETH and a total value locked (TVL) of 100 ETH, a user supplying 1 ETH would incur a fee of approximately 0.000001 ETH.

Transaction fees may also vary in accordance with the yield generated per unit time in the pool.
