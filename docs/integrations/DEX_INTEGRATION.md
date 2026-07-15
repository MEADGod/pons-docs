# DEX integration

PONS currently presents Uniswap as the launch market on Robinhood Chain.

## Trading integration

A DEX or router integration should determine from verified on-chain state:

- the Uniswap version;
- factory and router addresses;
- position manager and quoter addresses where applicable;
- pool address and fee tier;
- ETH/WETH handling; and
- token ordering and decimals.

Do not assume compatibility with a particular Uniswap deployment solely from the word "Uniswap" in the interface.

## Additional DEX support

The reviewed public interface does not publish a process for adding another DEX as a PONS launch target. Teams seeking integration should contact PONS through an official, verified channel and request technical requirements. Never send private keys, signing secrets, or privileged credentials.
