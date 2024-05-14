# Smart Contract Management

Overview 

This initiative showcases fundamental ATM operations on the Ethereum and Avalanche blockchains. It features a React interface for user interaction and a Solidity-based smart contract for ATM processes.

## Requirements
To interact with the smart contract, you'll need:
* A MetaMask wallet for Ethereum transactions.
* Access to Ethereum and Avalanche networks for smart contract deployment.
* A foundational grasp of the Ethereum and Avalanche blockchain frameworks.

## Usage
1. Install MetaMask for Ethereum transactions.
2. Launch the supplied Solidity smart contract on a suitable Ethereum or Avalanche network.
3. Link your MetaMask wallet to the active smart contract.
4. Utilize the React interfa

## Smart Contract Details 
The Solidity contract facilitates elementary ATM tasks such as deposits and withdrawals, with built-in error management for withdrawal attempts exceeding account balances.

Contract Name
* Name: Assessment

State Variables
* owner: An address with payment capabilities, denoting the contract initiator.
* balance: A numeric value tracking the contract’s funds.

Events
* Deposit: Signals the addition of funds.
* Withdraw: Indicates the deduction of funds.

Constructor
* Parameters: A starting balance.
* Function: Sets up the contract initiator and initial funds, with the capability to accept funds upon creation.
  
Functions
getBalance: Publicly accessible, it reveals the contract’s current funds.
* deposit: Open to the public, it allows the addition of a specified sum to the contract, restricted to the contract initiator.

* withdraw: Publicly accessible, it permits the contract initiator to retrieve a specified sum, barring withdrawals that surpass the available funds.
  

Custom Error
* Name: InsufficientBalance
* Function: An error triggered when a withdrawal request exceeds available funds.

## Deployment
* Begin by installing dependencies in the IDE terminal with npm i.
* Open two additional terminals and initiate npx hardhat node.
* Deploy the contract with npx hardhat run --network localhost scripts/deploy.js.
* Start the frontend with npm run dev, then navigate to the local server at http://localhost:3000/.

## Authors
Sean Ydna A. Abellanosa

## License
This project is licensed under the MIT License - see the LICENSE.md file for details
