# module-1---subnets

# ERC20 and Vault Contracts README

## Overview

This README provides a brief guide to understanding and using the ERC20 and Vault contracts. These contracts are designed for handling token transfers and storing assets securely in a decentralized manner.

## 1. ERC20 Contract

The ERC20 contract is a standard Ethereum-based token contract that handles token transfers and approvals. This contract follows the [ERC20 standard](https://eips.ethereum.org/EIPS/eip-20).

### Key Functions:
- **`totalSupply()`**: Returns the total supply of the token.
- **`balanceOf(address)`**: Shows the balance of a given address.
- **`transfer(address, uint256)`**: Transfers tokens to a specified address.
- **`approve(address, uint256)`**: Approves an address to spend a specific amount of tokens.
- **`transferFrom(address, address, uint256)`**: Allows an approved address to transfer tokens on your behalf.
- **`allowance(address, address)`**: Shows the amount of tokens that an address is allowed to spend on behalf of another address.

### Events:
- **`Transfer(address indexed from, address indexed to, uint256 value)`**: Logs transfers between addresses.
- **`Approval(address indexed owner, address indexed spender, uint256 value)`**: Logs approvals of spenders.

### Usage:
Deploy the contract and interact using the functions above for creating, transferring, and approving token transactions.

---

## 2. Vault Contract

The Vault contract is designed to securely store tokens and handle deposits and withdrawals. It works with ERC20 tokens and can be used for creating staking systems, pooled investments, or other DeFi use cases.

### Key Functions:
- **`deposit(uint256 amount)`**: Deposits a specified amount of tokens into the vault.
- **`withdraw(uint256 amount)`**: Withdraws a specified amount of tokens from the vault.
- **`balance()`**: Returns the total balance held in the vault.
- **`getUserBalance(address user)`**: Shows the balance of a particular user.

### Events:
- **`Deposit(address indexed user, uint256 amount)`**: Logs deposits into the vault.
- **`Withdraw(address indexed user, uint256 amount)`**: Logs withdrawals from the vault.

### Usage:
1. **Approve the Vault**: Before depositing, approve the Vault contract to spend your tokens using the `approve()` function from the ERC20 contract.
2. **Deposit Tokens**: Use the `deposit()` function to store tokens in the vault.
3. **Withdraw Tokens**: Call the `withdraw()` function to retrieve your tokens.
 
## Author

Narine 

narine765narine@gmail.com

