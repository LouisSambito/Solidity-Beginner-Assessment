# MY TOKEN
This Solidity program is a simple "My Token" program that demonstrates how to create and burn a Token on solidity.

## Description
This program is a simple contract written in Solidity, a programming language used for developing smart contracts on the Ethereum blockchain. The contract is designed to create a non-fungible token (NFT). This program serves as a straightforward introduction to Solidity programming and NFT creation, providing a foundational step towards more complex projects in the future.

## Getting Started 

### Executing program

To run this program, you can use Remix, an online Solidity IDE. To get started, go to the Remix website at https://remix.ethereum.org/.
Once you are on the Remix website, create a new file by clicking on the "+" icon in the left-hand sidebar. Save the file with a .sol extension (e.g., myToken.sol). Copy and paste the following code into the file:
pragma solidity 0.8.18;


contract MyToken {

    // public variables here
     string public tokenName = "META";
     string public tokenAbbrv = "MTA";
     uint public totalSupply = 0;

    // mapping variable here
   mapping(address => uint) public balances;

    // mint function
    function mint (address _address, uint _value) public{
        totalSupply += _value;
        balances[_address] += _value;
    }  
    
    // burn function
    function burn (address _address, uint _value) public{
        if (balances[_address] >= _value)
        totalSupply -= _value;
        balances[_address] -= _value;
    }
      

}

To compile the code, click on the "Solidity Compiler" tab in the left-hand sidebar. Make sure the "Compiler" option is set to "0.8.18" (or another compatible version), and then click on the "Compile myToken.sol" button.

Once the code is compiled, you can deploy the contract by clicking on the "Deploy & Run Transactions" tab in the left-hand sidebar. Select the "myToken" contract from the dropdown menu, and then click on the "Deploy" button.

Once the contract is deployed, you can interact with it by pressing and arrow at the bottom of "Deployed/Unpinned Contracts". Select "total supply" button to see how many tokens you have.
There is a drop donw button beside the "Burn button" click on it and put the account address. the account address is located at the top of "Deploy & Run Transaction" tab.

## Authors

Louis Sambito

## License

This project is licensed under the MIT License - see the LICENSE.md file for details








