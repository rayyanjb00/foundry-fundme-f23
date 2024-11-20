# FundMe Smart Contract

The `FundMe` smart contract allows users to contribute funds in ETH while ensuring a minimum contribution threshold is met, based on the current ETH/USD price. The contract owner can withdraw funds in an optimized way to minimize gas costs. 

This repository includes:
- A Solidity smart contract for crowdfunding (`FundMe.sol`).
- Unit and integration testing using tools like Foundry.
- Deployment and testing of the contract on the Ethereum mainnet/testnets as well as on zkSync.

---

## Features

### Core Functionalities
- **Funding**: Users can fund the contract, with a minimum threshold checked using Chainlink Price Feeds.
- **Withdrawals**: The contract owner can withdraw all funds, resetting the contract state.
- **Optimized Withdrawals**: A gas-efficient withdrawal function (`cheaperWithdraw`).

### Security
- **Ownership Restriction**: Functions like `withdraw` are restricted to the owner using a custom error `FundMe_NotOwner`.
- **Fallback Functions**: Handles ETH sent directly to the contract via the `fallback` and `receive` functions.

---

## Getting Started

### Prerequisites
- Node.js and npm
- Solidity development environment (Remix, Foundry, Hardhat, etc.)
- zkSync CLI and tools for L2 testing

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/rayyanjb00/foundry-fundme-f23.git
   cd foundry-fundme-f23


## Documentation

https://book.getfoundry.sh/

