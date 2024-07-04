
# CREATE A TOKEN

This Solidity project is a simple coin generator implemented in Solidity. The Purpose of this program is to teach how coins are created, mint, and burn.

## Description

This program is a simple contract written in Solidity, a programming language used for developing smart contracts on the Ethereum blockchain. This program has 3 function That let you mint and burn at the same time check the balane of your coin. $$ It allows users to mint and burn tokens, demonstrating the basic functionality of a token contract. The project is designed for beginners to understand the basics of Solidity and token operations using the Remix IDE.

## Getting Started

### Installing

To run this program, you can use Remix, an online Solidity IDE. To get started, go to the Remix website at https://remix.ethereum.org/

Once you are on the Remix website, create a new file by clicking on the "+" icon in the left-hand sidebar. Save the file with a .sol extension (e.g., myToken.sol).
contract MyToken {

    // public variables here
     string public tokenName = "META";
     string public tokenAbbrv = "MTA";
     uint public totalSupply = 0;

### Executing program

To interact with the smart contract in Remix IDE, follow these steps:

 **Compile the Contract**:
    - In the Remix IDE, navigate to the "Solidity Compiler" tab.
    - Ensure the compiler version matches the pragma version in `myToken.sol` (e.g., ^0.8.0).
    - Click "Compile myToken.sol".

 **Deploy the Contract**:
    - Navigate to the "Deploy & Run Transactions" tab.
    - Select "myToken" from the contract dropdown.
    - Click "Deploy".
    - The deployed contract will appear at the bottom under "Deployed Contracts".

 **Mint Tokens**:
    - Expand the deployed contract section.
    - Locate the `mint` function.
    - Enter the address and the amount of tokens to mint.
    - Click "Transact".

 **Burn Tokens**:
    - Locate the `burn` function.
    - Enter the address and the amount of tokens to burn.
    - Click "Transact".

 **Check Balance**:
    - Locate the `balanceOf` function.
    - Enter the address to check the balance.
    - Click "Call".



## Authors

Louis Sambito


## License

This project is licensed under the MIT License - see the LICENSE.md file for details





















