# Contract reference

PONS has not published a complete launchpad ABI or deployment registry in the reviewed public interface. This page therefore documents only safe standard read paths and the information still required for a full integration.

## Standard ERC-20 reads

```solidity
interface IERC20Metadata {
    function name() external view returns (string memory);
    function symbol() external view returns (string memory);
    function decimals() external view returns (uint8);
    function totalSupply() external view returns (uint256);
    function balanceOf(address account) external view returns (uint256);
    function allowance(address owner, address spender) external view returns (uint256);
}
```

These calls describe a token but do not prove that it was launched by PONS.

## Required PONS publication

A production-grade reference requires:

- official launch contract addresses and deployment blocks;
- verified source code and ABIs;
- canonical launch event and token-verification getter;
- pool and locker discovery methods;
- creator-fee getters and events;
- graduation calculation, getter, and event;
- admin, ownership, and upgrade model; and
- custom errors and launch restrictions, if any.

Never substitute interfaces from another launchpad. Function names and struct layouts are protocol-specific even when products look similar.
