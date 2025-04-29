
# 🚀 TrustFundr – Decentralized Startup Funding Platform
 
TrustFundr is a revolutionary decentralized platform that connects startups with investors in a secure, transparent, and milestone-based funding environment. By leveraging blockchain technology, we provide a trustless and verifiable platform where backers receive equity tokens in return for their funding, allowing them to have a stake in the growth of innovative new startups.

Unlike traditional funding platforms, TrustFundr empowers both startups and investors by using Ethereum smart contracts to ensure secure and milestone-based fund releases. Whether you're a startup looking to fund your next big idea or an investor looking to back the next game-changer, TrustFundr provides an efficient and transparent way to invest and grow together.

---

## 📚 Table of Contents

- [✨ Features](#-features)
- [🛠 Tech Stack](#-tech-stack)
- [🚀 Getting Started](#-getting-started)
  - [📦 Install Frontend (React)](#-install-frontend-react)
  - [🔗 Deploy Smart Contracts](#-deploy-smart-contracts)
  - [📦 Install Backend (Node.js) ](#-install-backend-nodejs)
- [⚠️ Disclaimers](#-disclaimers)

---

## ✨ Features

- 🛡️ **Smart Contract Based Milestone Fund Releases**  
  Funds are released to startups in predefined milestones, ensuring accountability, transparency, and progress tracking for both investors and founders.

- 💰 **Token/Equity in Exchange for Funds**  
  Investors receive equity tokens representing their share in the startup, providing them with a stake in the future success and growth of the funded project.

- 🧾 **DAO Governance for Investor Involvement**  
  Investors participate in the governance of the project through decentralized autonomous organization (DAO) mechanisms, ensuring community-driven decisions on project milestones and fund usage.

- 🔑 **Wallet-Based Authentication**  
  Use your MetaMask wallet for seamless login and interaction with the platform. No need for traditional sign-ups, as the blockchain handles authentication through wallet addresses.

- 🌐 **Global Accessibility**  
  TrustFundr is a decentralized platform, meaning anyone, anywhere in the world, can invest in and fund startups, making the process more accessible to a broader audience.

- 🔄 **Blockchain Transparency and Security**  
  All transactions and fund releases are recorded on the Ethereum blockchain, offering complete transparency and security for every step of the funding process.

- 🔧 **Backend-Ready**  
  Planned Node.js backend integration with MongoDB for storing off-chain data such as investor details, startup profiles, and funding analytics, enabling deeper insights and interaction.

- 📊 **Analytics and Reporting**  
  Investors and startups have access to detailed reports and analytics, helping them track progress and make informed decisions based on data-driven insights.

- 📈 **Scalable and Future-Proof**  
  Designed for future expansion, with plans to integrate additional blockchains, new features for startup growth, and enhanced governance systems to meet the evolving needs of investors and startups.

---


## 🛠 Tech Stack

- **Frontend**: React, Vite, Tailwind CSS
- **Blockchain**: Solidity, Hardhat, Sepolia Testnet
- **Wallet**: Metamask (wallet-based authentication)
- **Smart Contract Deployment**: Hardhat + Thirdweb RPC
- **Backend**: Node.js + Express + MongoDB

---

## 📂 Folder Structure
```bash
/
├── FE/                  # Frontend (React + Vite + TailwindCSS)
│   ├── public/          # Public assets (images, favicon, etc.)
│   ├── src/             # Source code for React app
│   │   ├── components/  # Reusable UI components
│   │   ├── context/     # Global state management (if using Context API)
│   │   ├── pages/       # Page components (Home, Dashboard, etc.)
│   │   ├── services/    # API calls, blockchain interactions, etc.
│   │   ├── styles/      # TailwindCSS custom styles
│   │   ├── App.js       # Main React component
│   │   └── index.js     # Entry point for React app
│   ├── .env             # Frontend environment variables (API URLs, etc.)
│   ├── package.json     # Frontend dependencies and scripts
│   └── vite.config.js   # Vite configuration for frontend build
├── BE/                  # Backend (Hardhat + Contracts + Node.js)
│   ├── contracts/       # Smart contracts (Solidity files)
│   ├── migrations/      # Smart contract migration scripts
│   ├── scripts/         # Deployment and interaction scripts
│   ├── server/          # Node.js backend (for off-chain storage, APIs, etc.)
│   │   ├── controllers/ # Backend logic to handle requests
│   │   ├── models/      # Mongoose models (if using MongoDB)
│   │   ├── routes/      # API route definitions
│   │   ├── services/    # Business logic (interact with smart contracts, DB, etc.)
│   │   ├── .env         # Backend environment variables (DB connection, secrets, etc.)
│   │   ├── app.js       # Express server setup
│   │   └── package.json # Backend dependencies and scripts
│   ├── hardhat.config.js # Hardhat configuration (network, compiler, etc.)
│   ├── .env             # Backend environment variables (network, private key, etc.)
│   ├── package.json     # Backend dependencies and scripts
│   └── README.md        # Backend-specific documentation
├── README.md            # Main project documentation (this file)
├── LICENSE.md           # Project license
└── .gitignore           # Git ignore file (for node_modules, .env, etc.)
```
---

## 🚀 Getting Started

### Prerequisites

- Node.js & npm
- Metamask wallet (Download from chrome web store)
- Sepolia ETH (get from [faucet](https://sepoliafaucet.com/))
- Git

---

### 📦 Install Dependencies

#### Frontend

```bash
cd FE
npm install
```

#### Backend (Smart Contracts)

```bash
cd BE
npm install
```

---

### 🧪 Compile & Deploy Smart Contracts
#### ⚠️ Disclaimer – No Need to Deploy Backend
Note:
You do not need to deploy the smart contracts yourself. The contracts are already deployed on the Sepolia testnet.
Just connect your Metamask wallet to the Sepolia network and interact with the existing contract.

Contract Address: 0xYourDeployedContractAddressHere

Network: Sepolia Testnet

Chain ID: 11155111

Only the developer (me) needs the .env and PRIVATE_KEY to deploy or modify contracts.

Set your private key in `.env` in the BE folder:

```
PRIVATE_KEY=your_private_key
```

Then deploy:

```bash
npx hardhat run scripts/deploy.js --network sepolia
```

📦 Install Backend (Node.js)
```bash
cd server   # Assuming your Node.js backend will be inside the 'server' folder
npm install
```
To run the backend server:
```bash
npm start   # or: node index.js / nodemon index.js
```
📌 Note: You will need to create a .env file in the server/ folder containing your MongoDB URI and any required environment variables.

---

### 💻 Run Frontend

```bash
cd FE
npm run dev
```

> App runs on: `http://localhost:5173/`
 
 ----

## 📷 Screenshots

![Screenshot 1](<client/public/images/SS1.png>)
![Screenshot 2](<client/public/images/SS2.png>)
![Screenshot 3](<client/public/images/SS3.png>)

---

## 🤝 Contributing

PRs are welcome. Feel free to open issues and suggestions.

---

## 👨‍💻 Author

**Vedant Srivastava** – CSE @ [LNCT BHOPAL] (0103CS221442)
**Email** - vedantsrivastava42@gmail.com

