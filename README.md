# Proveably Random Raffle Contracts

## About

A decentralized and verifiably fair lottery system built with Solidity, tested using Foundry, and powered by Chainlink VRF v2.5 and Chainlink Automation. This project simulates a real-world lottery where users can enter with ETH, and a random winner is picked after fixed intervals using Chainlink's provably random number generator.

## What does this contract do ?

1. Users can enter the lottery by paying for a ticket
    1. The ticket fees are going to go to the winner during the draw
2. After X period of time, the lottery will automatically draw a winner
    1. And this will be done programatically
3. Using Chainlink VRF & Chainlink Automation
    1. Chainlink VRF -> Randomness
    2. Chainlink Automation -> Time based trigger

## 🛠 Built using 

-  **Foundry**: development, testing, and deployment
-  **Solidity**: Writing Smart Contracts
-  **Chainlink VRF v2.5**: To generate provably random numbers on-chain
-  **Chainlink Automation**: Automatically triggers winner selection based on time intervals and contract state.
-  **Alchemy / Infura**: for RPC access to Sepolia testnet

## ⚙️ Requirements

### Foundry 

Documentation - https://book.getfoundry.sh/

### .env file should contain

```
SEPOLIA_RPC_URL=https://sepolia.infura.io/v3/your_project_id
MAINNET_RPC_URL=https://mainnet.infura.io/v3/your_project_id
PRIVATE_KEY=your_private_key
```

## 🧪 Usage

### 1.  **Clone the repository**:

    ```bash
    git clone [https://github.com/yourusername/foundry-smart-contract-lottery](https://github.com/yourusername/foundry-smart-contract-lottery)
    cd foundry-smart-contract-lottery
    ```

### 2.  **Install dependencies**:

    ```bash
    make install
    ```

### 3. **Build Contracts**:

    ```bash
    make build
    ```

### 4. **Run Tests**:

    ```bash
    make test
    ```

### 5. **Deploy locally (Anvil)**:

    ```bash
    make deploy
    ```

### 5. **Deploy to Sepolia**:

    ```bash
    make deploy-sepolia
    ```