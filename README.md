
# Avalanche Subnet Project

This repository contains Solidity smart contracts for an ERC20 token and a Vault contract. The ERC20 token contract implements standard functions such as  `transfer`,  `approve`,  `transferFrom`,  `mint`, and  `burn`. It also includes events for  `Transfer`  and  `Approval`. The Vault contract interacts with the ERC20 token contract, allowing users to deposit tokens and withdraw them later.

## ERC20 Token Contract

The ERC20 token contract named "Buzor Token" has a total supply of tokens and allows for transfers, approvals, and token mints and burns. The contract uses the OpenZeppelin's SafeMath library for safe arithmetic operations.

### Functions

-   `transfer`: Transfers a certain amount of tokens from the message sender to a recipient.
-   `approve`: Approves a certain amount of tokens to be spent by a spender.
-   `transferFrom`: Transfers a certain amount of tokens from a sender to a recipient using allowances.
-   `mint`: Mints a certain amount of tokens and assigns them to the message sender.
-   `burn`: Burns a certain amount of tokens from the message sender.

## Vault Contract

The Vault contract interacts with the ERC20 token contract. It allows users to deposit tokens into the vault and withdraw them later. The vault keeps track of the total supply of shares and the balance of shares owned by each user.

### Functions

-   `deposit`: Deposits a certain amount of tokens into the vault and mints an equivalent amount of shares.
-   `withdraw`: Withdraws a certain amount of tokens from the vault by burning an equivalent amount of shares.

## Interface

The IERC20 interface provides a standard interface for interacting with the ERC20 token contract. It includes functions for querying the total supply, balance of an account, transferring tokens, checking allowances, approving allowances, and transferring tokens from one account to another.