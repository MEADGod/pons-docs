# Security and risk

## For users

- Verify the domain is `pons.family` before connecting a wallet.
- Confirm Robinhood Chain and every transaction field in the wallet.
- Identify tokens by contract address, not name or ticker.
- Treat token images, descriptions, and links as untrusted content.
- Verify creator-wallet addresses before launching.
- Review developer-buy size and resulting ownership concentration.
- Inspect approvals and revoke obsolete allowances.
- Use deliberate slippage and avoid signing unexplained transactions.
- Expect extreme volatility, MEV, failed transactions, and network congestion.
- Do not treat graduation or locked launch liquidity as an endorsement.

## For integrators

- Require verified PONS addresses, source, ABIs, and deployment blocks.
- Verify the Uniswap pool, version, fee tier, router, and pair asset.
- Verify fixed-supply and liquidity-lock claims from bytecode.
- Sanitize and proxy remote metadata safely.
- Handle reorganizations, duplicate logs, RPC failures, and indexer lag.
- Use integer arithmetic for token amounts and fees.
- Separate read-only infrastructure from transaction signers.
- Monitor privileged roles and implementation changes.

## Responsible disclosure

Report vulnerabilities through an official PONS channel before public disclosure. Include the affected chain and contracts, reproduction steps, impact, and a minimal proof of concept. Never test with third-party funds or exceed what is necessary to validate the issue.

## Documentation limitations

This repository is not a smart-contract audit. The reviewed public PONS interface does not publish complete contracts, ABIs, deployment blocks, pool parameters, fee percentages, graduation logic, or admin/upgrade details. These must be verified before a production integration is considered complete.
