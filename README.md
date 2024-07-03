## Introduction

This project is a simple coin generator implemented in Solidity. It allows users to mint and burn tokens, demonstrating the basic functionality of a token contract. The project is designed for beginners to understand the basics of Solidity and token operations using the Remix IDE.

## Features

- **Mint Tokens**: Generate new tokens and add them to a specified address.
- **Burn Tokens**: Destroy tokens from a specified address, reducing the total supply.

## Installation

To get started with this project, follow the steps below:

 **Open Remix IDE**:
    - Go to [Remix IDE](https://remix.ethereum.org/).
    - Click on the file explorer icon on the left sidebar.
    - Click on the "Load a local file" button and select the `myToken.sol` file from the cloned repository.

## Usage

To interact with the smart contract in Remix IDE, follow these steps:

1. **Compile the Contract**:
    - In the Remix IDE, navigate to the "Solidity Compiler" tab.
    - Ensure the compiler version matches the pragma version in `myToken.sol` (e.g., ^0.8.0).
    - Click "Compile myToken.sol".

2. **Deploy the Contract**:
    - Navigate to the "Deploy & Run Transactions" tab.
    - Select "myToken" from the contract dropdown.
    - Click "Deploy".
    - The deployed contract will appear at the bottom under "Deployed Contracts".

3. **Mint Tokens**:
    - Expand the deployed contract section.
    - Locate the `mint` function.
    - Enter the address and the amount of tokens to mint.
    - Click "Transact".

4. **Burn Tokens**:
    - Locate the `burn` function.
    - Enter the address and the amount of tokens to burn.
    - Click "Transact".

5. **Check Balance**:
    - Locate the `balanceOf` function.
    - Enter the address to check the balance.
    - Click "Call".

## Smart Contract Overview

The main contract in this project is `myToken.sol`. Here's a brief overview of its structure and functions:

- **Variables**:
    - `balances`: A mapping to store token balances of addresses.
    - `totalSupply`: An integer to track the total supply of tokens.

- **Functions**:
    - `mint(address to, uint amount)`: Mints `amount` tokens to the `to` address.
    - `burn(address from, uint amount)`: Burns `amount` tokens from the `from` address.
    - `balanceOf(address account)`: Returns the token balance of the `account`.

## Testing

Testing can be performed within Remix IDE by invoking contract functions and checking the state changes. For automated testing, you can write tests in JavaScript or Solidity and run them using a framework like Hardhat or Truffle.

## Author

Loui Sambito

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
