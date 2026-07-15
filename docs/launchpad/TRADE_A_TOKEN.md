# Trade a token

PONS token pages surface launched fixed-supply assets and their Uniswap market on Robinhood Chain.

## Before trading

- Confirm Robinhood Chain is selected in the wallet.
- Verify the token contract address, not only its name or ticker.
- Confirm the pair asset and Uniswap pool.
- Inspect liquidity, holder concentration, price impact, and recent activity.
- Treat images, descriptions, and social links as untrusted user content.

## Execution

Review the exact token addresses, input amount, estimated output, slippage, deadline, recipient, approval spender, and gas in the wallet. A quote is indicative only; pool state can change before execution.

## Approvals

Token sales may require an ERC-20 allowance. Confirm that the spender belongs to the intended Uniswap router deployment and avoid unlimited approvals unless they are necessary and understood. Revoke obsolete allowances when appropriate.

## Canonical state

The interface can use indexed data for discovery and display. The blockchain transaction and verified pool state remain authoritative for execution.
