# Liquidity Module

The Liquidity Module is responsible for all farming operations within Birdie. It is composed of various Single Token Vaults and Pair Token Vaults that connect to protocols offering diversified yield opportunities for each token. Through this Liquidity Module, users can easily engage in both Single Token Farming and Pair Token Farming.

<figure><img src="../../.gitbook/assets/스크린샷 2024-06-20 오후 1.34.42.png" alt=""><figcaption></figcaption></figure>

* Single Token Farming: This service leverages lending protocols or similar mechanisms to generate yield from individual tokens, much like first-generation Yield Farming Aggregators. The system automatically harvests rewards at set intervals and reinvests them, enabling the power of compounding.
* Pair Token Farming: In this model, receipt tokens corresponding to each individual token are paired and supplied as liquidity to a chosen DEX. As a result, users earn both the yield from Single Token Farming and the trading fee income from the paired tokens. This service also supports automated harvesting and reinvestment to realize compound returns.



### Multi-Token Reward–Enabled Vault

Birdie’s vaults support Multi-Token Rewards—in other words, they enable the distribution of several types of tokens as rewards. Depending on the token, timing, or operational strategy, users may receive additional yield opportunities through the allocation of multiple tokens as rewards.

