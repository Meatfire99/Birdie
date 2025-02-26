# Swap

The Swap service provided by Birdie is not an independently operated AMM DEX. Rather, it leverages liquidity supplied via the Liquidity Module to conduct transactions on a rigorously vetted DEX. However, as with conventional AMMs, the user must hold tokens that are paired for the swap.

Since liquidity supplied through Birdie consists of receipt tokens obtained from depositing assets into an underlying protocol, a swap would conventionally require that the user obtains the corresponding receipt tokens from that same protocol.

To simplify this complex process, Birdie offers the Swap Module.

<figure><img src="../../.gitbook/assets/스크린샷 2024-06-25 오후 2.09.45.png" alt=""><figcaption></figcaption></figure>

1. Through a virtual DEX interface provided by Birdie, the user selects the token they hold and the desired token to receive, then enters the swap amount. From the user’s perspective, both the token being exchanged and the token received are native tokens.
2. As with any conventional DEX (such as Uniswap), the user first authorizes the token usage.
3. Once the authorization is complete, the Swap button is activated. For explanatory purposes, let us denote the token held by the user as Token1 and the token to be received as Token2.
4. The Swap Module accepts Token1 and deposits it via the corresponding Single Token Vault (Vault1) into the underlying protocol’s Token1 pool, receiving a receipt token (Receipt Token1) and issuing a corresponding Birdie receipt token.
5. The Birdie receipt token for Token1 is then exchanged within the liquidity pool for the Birdie receipt token corresponding to Token2.
6. This exchanged Birdie receipt token is then converted back (via the appropriate Single Token Vault, Vault2) into Receipt Token2, which is subsequently redeemed from the underlying protocol’s Token2 pool as Native Token2.
7. Native Token2 is finally transferred to the user, completing the swap process.
8. The user can then verify the received amount of Token2 in their connected wallet.

Though the process is complex, Birdie’s automation ensures that the only manual steps are the initial configuration, token approval, and the final button click—keeping the overall user experience straightforward and user-friendly.&#x20;
