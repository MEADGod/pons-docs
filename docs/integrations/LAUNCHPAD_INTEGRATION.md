# Launchpad integration

This guide is for wallets, explorers, trading tools, analytics, and notification services integrating PONS launches.

## 1. Establish trusted deployments

Obtain the official PONS launch contracts, verified source, ABIs, and deployment blocks. The public interface reviewed on 15 July 2026 does not provide a complete registry, so a production indexer should not begin from guessed addresses.

## 2. Discover launches

Once a verified launch event is published, index it from the official deployment block and store `(chainId, transactionHash, logIndex)` as the event key. Handle reorganizations, duplicates, bounded log ranges, RPC timeouts, and confirmation depth.

Until then, PONS interface data may assist discovery but should not be treated as canonical proof that a token is an official launch.

## 3. Verify and enrich

For each token:

1. verify the launch transaction and deployer path;
2. read ERC-20 name, symbol, decimals, total supply, and bytecode;
3. resolve the actual Uniswap pool and pair asset;
4. verify the liquidity lock on-chain;
5. obtain creator wallet and graduation state from verified contracts; and
6. treat images, descriptions, and links as untrusted content.

## 4. Quote and trade

Use the verified Uniswap router and quoter for Robinhood Chain. Resolve the pool version and fee tier on-chain, simulate the transaction, and make slippage, deadline, recipient, and allowance explicit.

## Production checklist

- [ ] Official PONS addresses and deployment blocks verified.
- [ ] ABI and bytecode pinned.
- [ ] Reorganization and duplicate handling implemented.
- [ ] Fixed-supply assumptions verified from bytecode.
- [ ] Pool, pair asset, version, and fee tier verified.
- [ ] Liquidity-lock contract and withdrawal properties verified.
- [ ] Creator-fee and graduation logic verified.
- [ ] Metadata sanitized and size-limited.
- [ ] On-chain state used for execution-critical values.
