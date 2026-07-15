# Trading safeguards

The reviewed PONS interface does not publish launch-block restrictions, max-wallet rules, max-transaction limits, transfer taxes, or an anti-snipe window.

## Integration rule

Do not assume that restrictions exist or do not exist solely from the UI. Before production support:

1. obtain the verified token implementation and ABI;
2. inspect transfer logic and custom errors;
3. simulate buys, sells, and transfers;
4. test launch-block and early-block behavior; and
5. monitor implementation or configuration changes.

## Safe user behavior

- Simulate transactions where possible.
- Use deliberate slippage and deadline values.
- Verify approvals and recipients.
- Expect MEV, price movement, failed transactions, and network congestion.
- Do not increase slippage automatically after an unexplained revert.
