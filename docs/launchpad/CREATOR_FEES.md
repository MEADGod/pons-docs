# Creator fees

The PONS launch form states that the creator wallet receives creator fees. It does not publish a universal creator-fee percentage, accrual formula, claim ABI, or distribution schedule in the reviewed interface.

## Creator wallet

- By default, the connected wallet is used.
- A different EVM address can be entered in Advanced settings.
- The same destination is described as receiving the developer-buy tokens.

Verify the destination address before launch. A typo or inaccessible address may permanently redirect proceeds.

## Integration guidance

Do not hard-code an assumed fee percentage or claim method. A production integration should use verified contract source, ABI, and live configuration supplied by PONS. Display gross accrual, protocol allocation, creator allocation, claimable amount, and gas separately whenever those values become available.
