# Swap Module

In an AMM-based DEX, liquidity pools for both the token to be exchanged and its paired counterpart must exist. For example, exchanging ETH for USDT necessitates an ETH-USDT liquidity pool.

While it is feasible to deposit assets into interest-bearing protocols via the Liquidity Module and then supply liquidity on a DEX using the resulting receipt tokens, trading within such pools requires that the user holds the corresponding receipt tokens in the correct pairing. Without them, no trade can occur—liquidity is merely supplied without generating fee income.

To resolve this, Birdie has developed a virtual DEX—the Swap Module. This module converts the value of the receipt tokens supplied via the Liquidity Module back into their original token equivalents based on the current exchange rate. Consequently, users can swap tokens just as they would on a conventional DEX. When a user initiates a swap with a native token, the Swap Module deposits that token into the underlying protocol to generate receipt tokens, executes the swap within the liquidity pool, and then redeems the swapped receipt tokens back into the native token. Though the process is intricate, it is fully automated, and the user experience remains as straightforward as using any standard DEX.

While the automated process involves a more complex sequence of transactions—resulting in slightly higher gas fees compared to typical DEX trades—the enhanced yield potential and sufficient liquidity (which helps to reduce slippage) serve to offset these costs. Moreover, the Birdie team intends to implement various incentives to further promote swap transactions.



### Growing and Expanding Liquidity Automatically

Typically, when liquidity is supplied to a DEX, the overall size of the liquidity pool remains static unless additional funds are provided. Although trading may change the exchange rate and accrue fee income to liquidity providers, the pool’s size itself remains largely unchanged unless reinvested through yield farming aggregators.

In contrast, liquidity supplied through Birdie continually grows in line with the yields from the underlying Single Token Farming protocols. While identical interest rates might leave the exchange rate unchanged, differing rates among tokens will cause the exchange rate to adjust as their values increase. Furthermore, as trading fee income is automatically harvested and reinvested (at the updated exchange rate), the liquidity pool’s size increases. This expanding liquidity not only creates opportunities for arbitrage but also incentivizes swap transactions that further generate fee income.
