# Launch a token

## Launch flow

1. Open the official PONS creation page.
2. Connect an EVM wallet on Robinhood Chain.
3. Upload a token image accepted by the form.
4. Enter the token name and ticker. The interface displays the ticker with a `$` prefix.
5. Add an optional description and community links.
6. Optionally configure a developer buy.
7. Leave the creator wallet empty to use the connected wallet, or enter another valid EVM address.
8. Review the launch fee, graduation target, liquidity status, and wallet transaction.
9. Confirm the transaction and record the deployed token contract address.

## Token details

- **Name:** full token name shown in the interface.
- **Ticker:** short token symbol; enter it without the `$` prefix.
- **Description:** optional project summary.
- **Token image:** image used by the interface.
- **X profile:** optional X handle.
- **Telegram:** optional Telegram community.
- **Website:** optional project website in Advanced settings.

The public form reviewed on 15 July 2026 does not display field-length, image-dimension, or file-size limits before upload. Treat client-side validation as authoritative and do not document guessed limits.

## Advanced settings

### Creator wallet

The creator wallet receives creator fees and the tokens resulting from the developer buy. Leave the field empty to use the currently connected wallet. If another address is provided, verify it carefully before signing; blockchain transfers may be irreversible.

### Developer buy

The developer buy is optional and denominated in ETH. It purchases part of the launched token during the launch flow. Review the amount and resulting ownership concentration before confirming.

## Current launch summary

The public interface currently displays:

- DEX: Uniswap;
- pair asset: ETH;
- launch fee: `0.0005 ETH`;
- graduation target: `4.2 ETH`; and
- liquidity: locked.

These are live interface values, not permanent constants. Confirm them at launch time.

## Example launch

For example, a fictional token could be configured as follows:

- **Image:** an image accepted by the launch form.
- **Name:** `RobinHat`.
- **Ticker:** `RHAT`, displayed as `$RHAT`.
- **Description:** `A community token for people who always wear a robinhood hat.`
- **Community links:** optional and may be left empty.
- **Creator wallet:** left empty to use the connected wallet, or set to another verified EVM address.
- **Developer buy:** optional; enter an ETH amount or leave it at zero.

Names and tickers are not unique identifiers. Users should verify Hatcoin by its deployed contract address rather than its name or `$HATCOIN` ticker alone.
