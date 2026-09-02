[LAUNCH_TOKEN.md](https://github.com/user-attachments/files/31722064/LAUNCH_TOKEN.md)
# Launch a Token

## Launch Flow

1. Open the official PONS creation page.
2. Connect an EVM wallet on Robinhood Chain.
3. Upload a token image accepted by the creation form.
4. Enter the token name and ticker. Enter the ticker without the `$` prefix; the interface adds it automatically.
5. Add an optional description and community links.
6. Optionally configure a developer buy.
7. Leave the creator wallet field empty to use the connected wallet, or enter another valid EVM address.
8. Review the launch fee, graduation target, liquidity status, developer-buy amount, and wallet transaction.
9. Confirm the transaction.
10. Record the deployed token contract address and use it as the token's canonical identifier.

## Token Details

- **Name:** Full token name displayed in the interface.
- **Ticker:** Short token symbol entered without the `$` prefix.
- **Description:** Optional project summary.
- **Token image:** Image displayed on the token page.
- **X profile:** Optional X account or handle.
- **Telegram:** Optional Telegram community link.
- **Website:** Optional project website available under Advanced settings.

The public form reviewed on 15 July 2026 did not display field-length, image-dimension, or file-size limits before upload. Treat the form's current client-side validation as authoritative and do not document guessed limits.

## Advanced Settings

### Creator Wallet

The creator wallet receives creator fees and any tokens resulting from the developer buy.

Leave the field empty to use the currently connected wallet. If another address is provided, verify it carefully before signing. Blockchain transactions and transfers may be irreversible.

### Developer Buy

The developer buy is optional and denominated in ETH. It purchases part of the launched token during the launch flow.

Before confirming, review:

- the ETH amount;
- the estimated token amount;
- the resulting ownership concentration;
- the total transaction cost; and
- the selected creator wallet.

Leave the developer-buy amount at zero if no initial purchase is required.

## Current Launch Summary

The public interface currently displays:

- **DEX:** Uniswap
- **Pair asset:** ETH
- **Launch fee:** 0.0005 ETH
- **Graduation target:** 4.2 ETH
- **Liquidity:** Locked

These are live interface values, not permanent protocol constants. Confirm every value directly in the launch interface before signing.

## Example Launch: Reddit Chair Coin

A fictional example token could be configured as follows:

- **Image:** A Reddit Chair Coin image accepted by the launch form.
- **Name:** Reddit Chair Coin
- **Ticker:** `RCHAIR`, displayed as `$RCHAIR`
- **Description:** Reddit chair paired to Reddit pairs.
- **X profile:** Optional and may be left empty.
- **Telegram:** Optional and may be left empty.
- **Website:** Optional and may be left empty.
- **Creator wallet:** Leave empty to use the connected wallet, or provide another verified EVM address.
- **Developer buy:** Enter an ETH amount or leave it at zero.

This example is fictional and does not represent a deployed token, verified project, or financial opportunity.

Names and tickers are not unique identifiers. Users should verify Reddit Chair Coin using its deployed contract address rather than relying only on the name **Reddit Chair Coin** or the `$RCHAIR` ticker.
