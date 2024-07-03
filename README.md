# Degen Token (DGN)

Degen (DGN) is an ERC20 token contract created using the OpenZeppelin library. This token is burnable and has no decimal places.

## Features

- **Mintable:** Only the contract owner can mint new tokens.
- **Burnable:** Tokens can be burned by the owner.
- **No Decimals:** The token does not support fractional units.

## Getting Started

### Prerequisites

To interact with this contract, you need the following installed:

- [Node.js](https://nodejs.org/)
- [Hardhat](https://hardhat.org/)
- [MetaMask](https://metamask.io/)

### Installation

1. **Clone the repository:**
   ```bash
   git clone <repository_url>
   cd <repository_directory>
Install dependencies:
npm install
Compile the contract:
npx hardhat compile
Deployment
To deploy the contract, you need to set up your environment variables with your private key and Infura or Alchemy API key.
Create a .env file:
touch .env
Add your environment variables to .env:
Get Balance
To get the balance of your account, call the getBalance function.
const balance = await degenContract.getBalance();
console.log(`Your balance: ${balance}`);
Transfer Tokens
To transfer tokens to another address, use the transferToken function.
await degenContract.transferToken(receiverAddress, amount);
Burn Tokens
To burn tokens from your account, call the burnTokens function.
await degenContract.burnTokens(amount);
Contract Details
Solidity Version
The contract is written in Solidity ^0.8.20.

Importing OpenZeppelin Contracts
The contract uses the following OpenZeppelin Contracts:

ERC20
ERC20Burnable
Ownable
Contract Methods
mint(address to, uint256 amount): Mints amount tokens to the to address. Only callable by the owner.
decimals(): Returns the number of decimal places the token uses, which is 0.
getBalance(): Returns the token balance of the caller.
transferToken(address receiver, uint256 amount): Transfers amount tokens to the receiver address.
burnTokens(uint256 amount): Burns amount tokens from the caller's balance.
License
This project is licensed under the MIT License - see the LICENSE file for details.

Acknowledgments
OpenZeppelin for the ERC20 standard implementation and utilities.
Disclaimer
Use this contract at your own risk. The author is not responsible for any loss of funds or damage caused by using this contract.

Feel free to adjust the content according to your specific requirements and details for the repository.

