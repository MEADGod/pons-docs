# PONS Documentation

Developer and user documentation for **PONS**, a non-custodial launchpad for fixed-supply tokens on Robinhood Chain.

PONS lets creators launch tokens, optionally make a developer buy, direct creator proceeds to a selected wallet, and make the token available through a Uniswap market. The launch interface currently displays a `0.0005 ETH` launch fee, a `4.2 ETH` graduation target, and locked liquidity.

> **Status:** Documentation snapshot verified against the public PONS launchpad on 15 July 2026. Interface values and protocol configuration can change. Always verify the transaction shown by your wallet before signing.

## Documentation

- [Introduction](docs/getting-started/INTRODUCTION.md)
- [Quickstart](docs/getting-started/QUICKSTART.md)
- Launchpad
  - [Overview](docs/launchpad/OVERVIEW.md)
  - [Launch a token](docs/launchpad/LAUNCH_A_TOKEN.md)
  - [Trade a token](docs/launchpad/TRADE_A_TOKEN.md)
  - [Creator fees](docs/launchpad/CREATOR_FEES.md)
  - [Graduation](docs/launchpad/GRADUATION.md)
- Concepts
  - [How launches work](docs/concepts/HOW_LAUNCHES_WORK.md)
  - [Liquidity and pricing](docs/concepts/LIQUIDITY_AND_PRICING.md)
  - [Trading safeguards](docs/concepts/TRADING_RESTRICTIONS.md)
- Contracts
  - [Deployments](docs/contracts/DEPLOYMENTS.md)
- Integrations
  - [Launchpad integration](docs/integrations/LAUNCHPAD_INTEGRATION.md)
  - [DEX integration](docs/integrations/DEX_INTEGRATION.md)
- Reference
  - [Contract reference](docs/reference/CONTRACT_REFERENCE.md)
  - [Chain](docs/reference/CHAINS.md)
  - [Fees](docs/reference/FEES.md)
  - [FAQ](docs/reference/FAQ.md)
  - [Glossary](docs/reference/GLOSSARY.md)
- [Security and risk](docs/security/SECURITY_AND_RISK.md)

## Quick facts

- Robinhood Chain launchpad.
- Fixed-supply token launches.
- Uniswap market with ETH as the displayed pair asset.
- Current displayed launch fee: `0.0005 ETH`.
- Current displayed graduation target: `4.2 ETH`.
- Launch liquidity is displayed as locked.
- Optional developer buy and custom creator wallet.
- Non-custodial interface: the connected wallet submits every transaction.

## Official link

- Launchpad: <https://pons.family/launchpad>

## Disclaimer

PONS is an interface to blockchain transactions and does not custody user assets. User-created tokens are not automatically safe, reviewed, or endorsed. Smart contracts, wallets, tokens, liquidity pools, price movement, network congestion, and transaction failures carry substantial risk. Nothing in this repository is financial advice.
