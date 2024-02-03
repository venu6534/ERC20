#  Vault and ERC20 

## Overview

Welcome to the Solidity Vault and ERC20 Token Contracts repository. This collection includes two robust Solidity smart contracts: `Vault` and `ERC20`. The `Vault` contract is tailored for managing ERC20 tokens in a decentralized vault setting, while the `ERC20` contract is an implementation of the ERC20 standard with added minting and burning functionality.

## Vault Contract

### Description

The `Vault` contract serves as a secure decentralized vault where users can deposit and withdraw ERC20 tokens. It intelligently manages total supply and individual user balances, enabling users to seamlessly interact with their assets.

### Key Features

- **Deposit Functionality**: Users can deposit ERC20 tokens into the vault, minting shares proportional to their contribution.

- **Withdrawal Functionality**: Users can withdraw tokens by burning their shares, receiving an amount proportionate to the shares burned.

### Internal Logic

- **Minting Function (`_mint`)**: Privately mints shares, updating total supply and user balances accordingly.

- **Burning Function (`_burn`)**: Privately burns shares, adjusting total supply and user balances accordingly.

### Events

- **Transfer Event**: Emitted when tokens are transferred within the vault.

### How to Use

1. Deploy the `Vault` contract by specifying the ERC20 token address in the constructor.

2. Users can seamlessly interact with the contract by depositing and withdrawing tokens.

## ERC20 Contract

### Description

The `ERC20` contract is a comprehensive implementation of the ERC20 standard, enhancing the basic functionalities with additional minting and burning capabilities. Users can transfer tokens, approve spending, and execute transfers on behalf of others.

### Key Features

- **Transfer Functionality**: Allows users to transfer tokens to other addresses.

- **Approval Mechanism**: Permits users to grant approval for spending tokens on their behalf.

- **Minting and Burning Functions**: Provides flexibility in creating and destroying tokens, respectively.

### Events

- **Transfer Event**: Emitted when tokens are transferred.

- **Approval Event**: Emitted when approval is granted for spending tokens.

### How to Use

1. Deploy the `ERC20` contract to create a new ERC20 token.

2. Utilize standard ERC20 functions, including transferring, approval for spending, and minting/burning tokens.

## Author 

venu 

venu61393@gmail.com

## License

Both contracts are licensed under the MIT License.
