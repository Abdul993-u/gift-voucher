Gift Voucher Smart Contract

A simple Clarity smart contract that allows users to mint, send, and burn **non-transferable gift vouchers**.  
This contract is designed as a lightweight learning project for interacting with the Stacks blockchain using **Clarinet**.


Features

- Any user can **mint** a voucher for themselves.
- Users can **send vouchers** to other users.
- Users can **burn (destroy)** their own vouchers if no longer needed.
- Contract maintains:
  - Individual voucher balances
  - Total voucher supply

Requirements

- [Clarinet](https://github.com/hirosystems/clarinet) installed  
- A Stacks development environment (VS Code recommended)


File Structure


Functions Overview

| Function | Type | Description |
|---------|------|-------------|
| `mint (amount uint)` | `public` | Mint gift vouchers to the caller. |
| `send (recipient principal amount uint)` | `public` | Send vouchers to another user. |
| `burn (amount uint)` | `public` | Burn vouchers from caller’s balance. |
| `get-balance (user principal)` | `read-only` | View any user's voucher balance. |
| `get-total-supply` | `read-only` | Returns the total supply of vouchers. |


Running and Testing with Clarinet

1. Compile the contract
```sh
clarinet check
