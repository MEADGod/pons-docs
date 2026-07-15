# How launches work

## User-visible flow

```text
Creator
  | token details + optional developer buy
  v
PONS launch interface
  | prepares wallet transaction(s)
  v
Robinhood Chain
  | fixed-supply token + Uniswap market
  v
PONS explore and token pages
```

PONS is non-custodial: the connected wallet submits every transaction. The interface currently presents the resulting token as fixed supply, the market as Uniswap/ETH, the launch liquidity as locked, and graduation at a displayed `4.2 ETH` target.

## Identity and discovery

Token names and tickers can be duplicated. The deployed contract address is the canonical token identifier. A reliable discovery system should also record the chain ID, transaction hash, block number, deployer, pool address, and verified launch contract when those values are available.

## Internal implementation

The reviewed public interface does not expose a complete factory ABI, launch event, supply constant, pool fee tier, locker implementation, or atomic transaction sequence. Those details must not be inferred from another launchpad. Use verified PONS contracts and source releases when published.
