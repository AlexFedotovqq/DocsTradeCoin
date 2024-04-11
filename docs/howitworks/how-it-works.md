# Mina Smart Contract Overview

**Smart Contracts Overview:**
The Mina Smart Contracts enable the functionality of an Automated Market Maker (AMM) mechanism. The AMM facilitates market-making activities, allowing users to engage in trading and liquidity provision. The contracts support trading between two assets and employ the constant product AMM function for price determination.

**Automated Market Maker (AMM) Functionality:**
The AMM mechanism supports two types of users: traders and liquidity providers.

- **Traders:** Traders execute trades against liquidity pools.
- **Liquidity Providers:** Liquidity providers contribute assets to the liquidity pools.

**Constant Product AMM Function:**
The AMM mechanism utilizes the constant product AMM function for determining prices and facilitating trades. This function is represented by the formula:

```
b = (y * a) / (x + a)
```

Where:

- `b` represents the amount of token the user will receive.
- `a` represents the quantity of an asset that the user wishes to purchase.
- `x` and `y` represent the balances of two assets in the liquidity pool.

This formula allows users to compute the exact amount they need to pay to receive a certain quantity of an asset, based on the current state of the liquidity pool.

## Mina Smart Contract Documentation

**Smart Contracts Location:**
The smart contracts can be found in the following GitHub repository: [TradeCoin Smart Contracts](https://github.com/AlexFedotovqq/TradeCoin/tree/main/mina/src)

**Testing:**
To ensure the functionality and integrity of the smart contracts, a testing suite has been provided. These tests are located in the following GitHub repository: [TradeCoin Smart Contract Tests](https://github.com/AlexFedotovqq/TradeCoin/tree/main/mina/tests)

### Testing Procedure:

To test the smart contracts, follow these steps:

1. **Installation:**

   - Run `npm i` to install the necessary dependencies.

2. **Testing:**
   - Execute `npm test` to run the test suite.

## Other implemented functionality of TradeCoin contracts

### Signature Verification

Contracts within the TradeCoin ecosystem verify that transactions are intended by the user. This ensures the security and validity of transactions.

### One Direction Trades

The system supports trading one token for another in a single direction. This simplifies the trading process and ensures consistency within the ecosystem.

### Deposits and Withdrawals

Users can deposit and withdraw funds securely using the implemented functionality within the contracts. This feature enhances the usability and accessibility of the TradeCoin platform.

## Contract Overview

### BasicTokenContract

- **States:**
  - `totalSupply`: Tracks the number of minted tokens.
  - `admin`: Public key of the contract deployer.
- **Functionality:**
  - Implements basic token functionalities.
  - Admin signature required for access to methods.

### DexContract

- **States:**
  - `root`: Tracks the merkle tree root of the contract.
  - `admin`: Public key of the contract deployer.
  - `poolsTotal`: Total number of pools available.
- **Functionality:**
  - Acts as a router for available pools.
  - Creates and manages pools with unique PoolId struct.

### PairContract

- **States:**
  - `admin`: Public key of the contract deployer.
  - `tokenX` and `tokenY` addresses: Addresses of the token contracts.
  - `root`: Tracks the merkle tree root.
  - `userId`: Tracks the number of users enlisted in the pair.
- **Functionality:**
  - Whitelists users and manages personal balances.
  - Implements methods for modifying struct on application and smart contract levels.

### PairMintContract

- **States:**
  - `admin`: Public key of the contract deployer.
  - `reservesX`, `reservesY`: Reserves of tokens X and Y.
  - `reservesLPX`, `reservesLPY`: Reserves of LP tokens.
  - `totalSupplyLP`: Total supply of LP tokens.
- **Functionality:**
  - Tracks pair reserves and implements constant product AMM function for swaps.
  - Implements supply, withdrawal, mint, and burn methods for LP tokens.

## Testing

**Smart Contract Repositories:**

1. **Mina Smart Contracts:**

   - Repository: [TradeCoin Mina Smart Contracts](https://github.com/AlexFedotovqq/TradeCoin/tree/main/mina/src)
   - Instructions:
     - Clone the repository:
       ```
       git clone https://github.com/AlexFedotovqq/TradeCoin.git
       ```
     - Navigate to the Mina Smart Contracts directory:
       ```
       cd TradeCoin/mina/src
       ```
     - Install dependencies:
       ```
       npm install
       ```
     - Run tests:
       ```
       npm test
       ```
   - Highlights: Novel implementations include constant product AMM function for trades, signature verification, and one-way trades.

2. **Smart Contract Tests:**
   - Repository: [TradeCoin Smart Contract Tests](https://github.com/AlexFedotovqq/TradeCoin/tree/main/mina/tests)
   - Instructions:
     - Clone the repository:
       ```
       git clone https://github.com/AlexFedotovqq/TradeCoin.git
       ```
     - Navigate to the Smart Contract Tests directory:
       ```
       cd TradeCoin/mina/tests
       ```
     - Install dependencies:
       ```
       npm install
       ```
     - Execute tests:
       ```
       npm test
       ```
   - Coverage: Comprehensive test suite ensuring contract functionality and security.
   - By following these steps, you can thoroughly test the TradeCoin contracts and ensure their functionality and security in a blockchain environment.

**Frontend Repository:**

- Repository: [TradeCoin Frontend](https://github.com/AlexFedotovqq/TradeCoin/tree/main/my-app)
- Instructions:
  - Clone the repository:
    ```
    git clone https://github.com/AlexFedotovqq/TradeCoin.git
    ```
  - Navigate to the Frontend directory:
    ```
    cd TradeCoin/my-app
    ```
  - Install dependencies:
    ```
    yarn
    ```
  - Start the development server:
    ```
    yarn dev
    ```
