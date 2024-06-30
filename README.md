# Project-Degen-Token-ERC-20-Unlocking-the-Future-of-Gaming
# DegenToken

## Description

DegenToken is an ERC20 token smart contract deployed on the Avalanche network for Degen Gaming. This contract allows minting new tokens, transferring tokens between players, redeeming tokens for in-game items, checking token balances, and burning tokens when no longer needed.

## Getting Started

### Prerequisites

Ensure you have the following installed:

- Node.js
- npm

### Installation

1. Clone the repository:


   git clone https://github.com/your-username/DegenToken.git
Navigate to the project directory:


cd DegenToken
Install dependencies:


npm install
### Deploying the Contract
To deploy the DegenToken contract on the Avalanche Fuji testnet:

Configure your hardhat.config.js file with your private key and network details.

Compile the contracts:


npx hardhat compile
### Deploy the contract to Fuji testnet:


npx hardhat run scripts/deploy.js --network fuji
Interacting with the Contract
After deploying, you can interact with the contract:

### javascript

// Example code snippet to interact with DegenToken contract
const contract = await ethers.getContractAt("DegenToken", contractAddress);

// Transfer tokens
await contract.transferTokens(recipientAddress, amount);

// Mint new tokens
await contract.mint(recipientAddress, amount);

// Redeem tokens for an item
await contract.redeem(itemId, amount);

// Check token balance
const balance = await contract.checkBalance(accountAddress);

// Burn tokens
await contract.burn(amount);
Example Usage
Replace placeholders like contractAddress, recipientAddress, itemId, amount, and accountAddress with actual values relevant to your project.

### Authors
Prakhar Bhardwaj: https://github.com/prakhar4pb
### License
This project is licensed under the MIT License. See the LICENSE file for details.

