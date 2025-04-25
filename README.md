
# Whitelist Minting Core Contract


Whitelist minting is a crucial feature in many blockchain and NFT-based core projects. It refers to the process where only a specific group of pre-approved wallet addresses are allowed to mint tokens or NFTs during a designated time period. This process takes place before the public minting phase and is designed to ensure fairness, reduce congestion, and reward early supporters or contributors of a project.

In technical terms, the whitelist is a list of wallet addresses stored either on-chain or off-chain. The smart contract checks this list to verify whether a user is eligible to mint. If the address is not whitelisted, the contract denies minting access. This helps prevent issues like gas wars, bot attacks, and sudden spikes in transaction fees, which often occur during public mints.

Whitelist minting allows project teams to control supply and access more efficiently, ensuring that loyal community members get priority. It’s also commonly used in token launches, Initial Coin Offerings (ICOs), and DeFi projects to limit early access to trusted participants.

Overall, whitelist minting promotes a more secure, organized, and community-focused approach to launching new tokens or NFTs in the blockchain ecosystem.

---

## ⚙️ Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/HeadTarun/Whitelist-Minting-Core.git
cd Whitelist-Minting-Core
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Configure Environment Variables

Create a `.env` file in the project root:

```env
PRIVATEKEY="your_core_wallet_private_key"
CORE_TEST2_SCAN_KEY="your_testnet2_explorer_api_key"
```

> ⚠️ **Important:** Never share your private key or commit the `.env` file to version control.

---

## 🛠 Hardhat Commands

### Compile Contracts

```bash
npx hardhat compile
```

### Run Tests

```bash
npx hardhat test
```

### Deploy Contract

Use a deployment script:

```bash
npx hardhat run scripts/deploy.js --network core_testnet2
```

---

## 🔍 Contract Verification

You can verify contracts using Core block explorers:

```bash
npx hardhat verify --network core_testnet2 <deployed_contract_address> <constructor_args_if_any>
```

API keys for verification must be included in `.env` as shown above.

---