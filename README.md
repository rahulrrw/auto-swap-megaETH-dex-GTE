# 🔄 Auto Swap Bot (ETH ↔ cUSD) dex GTE on network megaETH

<img width="1280" height="559" alt="image" src="https://github.com/user-attachments/assets/664ed1c4-b597-480a-a6f3-c02ec46c9d60" />

---

## 🚀 Features
- Randomized daily swaps (number of transactions, amount per swap, and delay between swaps).
- Configurable RPC endpoint, wallet private key, and all randomization ranges via `.env`.
- Supports EIP-1559 transactions (`maxFeePerGas` & `maxPriorityFeePerGas`).
- Logs each swap with timestamp and transaction hash.
- Loop runs continuously every days once started.

---

## 📦 Installation
Clone the repository and install dependencies:

```bash
git clone https://github.com/abahuto/auto-swap-megaETH-dex-GTE.git
```
```bash
cd auto-swap-megaETH-dex-GTE
```
```bash
npm install
```

## ⚙️ Environment Setup
Create a .env file in the project root:
```bash
nano .env
```
Fill in your wallet details and randomization settings:
```bash
# RPC endpoint
RPC_URL=https://carrot.megaeth.com/rpc

# Private key (without quotes)
PRIVATE_KEY=your_private_key

# Wallet address
ADDRESS=your_address

# Contract addresses
ROUTER_ADDRESS=0xa6b579684e943f7d00d616a48cf99b5147fc57a5
WETH_ADDRESS=0x776401b9bc8aae31a685731b7147d4445fd9fb19
CUSD_ADDRESS=0xe9b6e75c243b6100ffcb1c66e8f78f96feea727f

# Random swap amounts (ETH → cUSD)
MIN_ETH=0.000001
MAX_ETH=0.00001

# Random swap amounts (cUSD → ETH)
MIN_CUSD=10
MAX_CUSD=20

# Random number of transactions per day
MIN_TX=34
MAX_TX=56

# Random delay between swaps (in seconds)
MIN_DELAY=60
MAX_DELAY=120
```

## ▶️ Running the Bot
To start the bot:
```bash
node index.js
```
What the bot does:

- Randomly decides between ETH → cUSD or cUSD → ETH swap each time.

- Executes a random number of swaps daily (within your configured range).

- Randomizes swap amount and delay between each transaction.

- Signs and sends transactions using your private key.

## 🔖 Tags
#eth #cusd #swap #bot #crypto #web3 #automation #trading #dex #evm #airdrop #megaETH #GTE
