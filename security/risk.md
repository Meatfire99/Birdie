# Risk

Yield farming is undertaken at the user’s sole risk. Due to issues arising either from Birdie itself or from the protocols it interacts with, users may experience partial or complete loss of their assets. The yields stated are not guaranteed. We strongly advise that users conduct thorough research and refrain from investing funds beyond their risk tolerance.



### Smart Contract Failure

Birdie’s smart contracts are open-source and have undergone extensive code reviews, testing, and third-party audits. They are not simply forks of pre-existing contracts. Although multiple audits have been successfully completed, such audits do not guarantee that Birdie’s target APY will be achieved or that the underlying protocols (or Birdie itself) will be impervious to hacking.



### Composability Risk

Birdie interacts with a variety of assets and multiple smart contracts. While such composability enhances Birdie’s functionality, any issue in one of the interacting contracts can expose the user to risk. Birdie strives to audit and evaluate the risks associated with the farming contracts, but the tokens involved in each strategy remain subject to inherent risks. Users are advised to examine the specific strategy of each vault before participating.



### Automated Market Maker Risk

Birdie employs yield farming strategies that expose liquidity to AMM-based DEXs. Providing liquidity in an AMM environment is a sophisticated endeavor and may incur losses in various ways. All actions are executed at the user’s own risk.

Impermanent Loss refers to the potential loss incurred when providing assets to a liquidity pool. Liquidity pools are used by decentralized exchanges such as Uniswap, Curve, and Balancer to facilitate the buying and selling of supported tokens. When converting funds to supply liquidity, fluctuations in the relative values of the assets in the AMM may result in partial or complete loss of value. Should even one asset in the pool depreciate significantly or become worthless, the entire pool’s position—regardless of the originally supplied assets—may experience a loss in value.

Moreover, if one asset appreciates in value relative to the others, holding the asset outside the pool may yield higher returns than supplying liquidity. It is imperative that users understand the mathematical principles behind impermanent loss before providing liquidity.



### Non-Liquidation (Temporary Illiquidity) Risk

In lending protocols, if all tokens deposited in a pool are borrowed—i.e., when a lending pool’s utilization rate reaches 100%—depositors may temporarily be unable to withdraw their assets.

Since Birdie utilizes lending protocols as the underlying mechanism to ensure stable interest income, there exists a risk that assets deposited via Birdie might be temporarily inaccessible in such scenarios.
