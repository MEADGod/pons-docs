# Supported chain

| Network | Chain ID | Native asset | Launch market | Graduation target |
|---|---:|---|---|---:|
| Robinhood Chain | `4663` | ETH | Uniswap | `4.2 ETH` |

PONS currently describes its launchpad as a Robinhood Chain product. Multi-chain support is not stated in the reviewed public launchpad.

Wallets and integrations should verify `eth_chainId == 0x1237` (`4663`) before constructing or signing a transaction. RPC endpoints, explorer URLs, and contract addresses should come from trusted current configuration.
