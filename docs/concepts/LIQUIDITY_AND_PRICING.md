# Liquidity and pricing

## Uniswap market

The PONS launch form identifies Uniswap and ETH for the launch market. Price is determined by the pool state, token ordering, decimals, liquidity distribution, and swap activity.

## Locked liquidity

The launch summary displays liquidity as locked. This statement should be limited to the PONS-created launch liquidity unless verified contracts prove a broader guarantee. Other parties may add independently owned liquidity positions with different withdrawal rights.

## Price and market capitalization

Market capitalization is a display metric derived from token price and supply. It is not the same as available liquidity and cannot generally be realized at the displayed price. Large trades can produce substantial price impact.

## Integration requirements

Implementations must correctly handle ERC-20 decimals, token ordering, the actual Uniswap version and fee tier, wrapped/native ETH presentation, and pool liquidity. PONS has not published those full technical parameters in the reviewed interface, so resolve them from verified on-chain contracts before routing trades.
