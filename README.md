MyToken Smart Contract

Overview

Welcome to the MyToken project! This project is a simple implementation of a custom token on the Ethereum blockchain using Solidity. The purpose of this project is to help students and beginners understand the basics of creating, minting, and burning tokens on the blockchain.

Features

Public Variables:
  - `tokenName`: Stores the name of the token (e.g., "SHIVKANT").
  - `tokenAbbrv`: Stores the abbreviation of the token (e.g., "SHIV").
  - `totalSupply`: Tracks the total supply of the tokens in circulation.
Mapping:
  - `balances`: A mapping to keep track of each address's token balance.
Functions:
  - `mint(address _address, uint _value)`: Increases the total supply and the balance of the specified address.
  - `burn(address _address, uint _value)`: Decreases the total supply and the balance of the specified address, ensuring the address has enough tokens to burn.

Prerequisites

Before you get started, you will need:
- A basic understanding of Solidity and smart contracts.
- An Ethereum wallet (like MetaMask) to interact with the contract.
- An Ethereum development environment (like Remix, Truffle, or Hardhat).

Installation and Setup

1. Clone the Repository:
   bash
   git clone https://github.com/yourusername/mytoken.git
   cd mytoken

2. Open the Project:
   - Open the project folder in Remix IDE or your preferred Ethereum development environment.

3. Compile the Contract:
   - Make sure the Solidity compiler version is set to `0.8.18` or higher.
   - Compile the `MyToken.sol` contract.

4. Deploy the Contract:
   - Deploy the contract using your local blockchain (like Ganache) or an Ethereum test network (like Rinkeby).
   - Make sure your Ethereum wallet has enough funds for deployment.

Usage

Minting Tokens

To mint new tokens, use the `mint` function. This function requires two parameters: the address to receive the tokens and the amount of tokens to be minted.

solidity
mint(address _address, uint _value)
address: The address that will receive the newly minted tokens.
value : The number of tokens to mint.

Burning Tokens

To burn tokens, use the `burn` function. This function requires two parameters: the address from which the tokens will be burned and the amount of tokens to be burned.
solidity
burn(address _address, uint _value)


address: The address from which the tokens will be burned.
value: The number of tokens to burn.

Note: The burn function includes a check to ensure the address has enough tokens to burn.

Example

Here’s an example of how you can interact with the contract after deployment:

1. Minting Tokens:
   Call the `mint` function with your address and the number of tokens you want to mint.
   solidity
   mint("0xYourEthereumAddress", 1000)
   

2. Burning Tokens:
   Call the `burn` function with your address and the number of tokens you want to burn.
   solidity
   burn("0xYourEthereumAddress", 500)
   

Contributing

This is a learning project, and contributions are welcome! If you have any suggestions or find any bugs, feel free to open an issue or submit a pull request.
License
This project is licensed under the MIT License. For more details, see the [LICENSE](LICENSE) file.

Acknowledgements

- Thanks to the Ethereum community for their excellent documentation and resources.
- Special thanks to all the developers and contributors who helped make Solidity and Ethereum so accessible.

