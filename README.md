
# Conclave

Conclave is a next-generation decentralized debate platform built on the Base blockchain. It empowers users to stake USDC, engage in meaningful debates, and let the community decide the outcome. Conclave is designed for transparency, fairness, and onchain reputation, bringing the spirit of open discourse to the web3 era.

---

## Table of Contents

- [Conclave](#conclave)
  - [Table of Contents](#table-of-contents)
  - [Features](#features)
  - [Architecture Overview](#architecture-overview)
  - [Folder Structure](#folder-structure)
  - [Tech Stack](#tech-stack)
  - [Getting Started](#getting-started)
    - [Prerequisites](#prerequisites)
    - [Installation](#installation)
  - [Usage](#usage)
    - [Running the App](#running-the-app)
    - [Environment Variables](#environment-variables)
  - [Smart Contracts](#smart-contracts)
  - [Contributing](#contributing)
    - [How to Contribute](#how-to-contribute)
  - [FAQ](#faq)
  - [License](#license)
  - [Contact](#contact)

---

## Features

- **Decentralized Debates:** Create, join, and participate in debates with real stakes.
- **Onchain Identity:** Use Basename for unique, verifiable onchain identities.
- **Staking Mechanism:** Stake USDC to participate and show conviction.
- **Community Voting:** Let the community determine the winning arguments.
- **Leaderboard & Reputation:** Track top debaters and build your onchain reputation.
- **Smart Wallet Integration:** Seamless wallet connection for secure transactions.
- **Modular Architecture:** Easily extend debate formats, voting mechanisms, and integrations.
- **Responsive UI:** Modern, accessible, and mobile-friendly interface.

---

## Architecture Overview

Conclave is composed of three main layers:

1. **Frontend (Next.js/React):** Provides the user interface, wallet connection, and interaction with smart contracts and backend APIs.
2. **Smart Contracts (Solidity/Foundry):** Handle debate creation, staking, voting, and reputation logic onchain.
3. **Backend/Database (Drizzle ORM, PostgreSQL):** Stores offchain data, user profiles, and supports advanced querying and analytics.

The platform leverages wagmi and Coinbase OnchainKit for wallet management and onchain interactions.

---

## Folder Structure

```
├── contracts/           # Solidity smart contracts and tests
│   ├── src/             # Main contract sources
│   ├── test/            # Contract tests
│   └── ...
├── public/              # Static assets
├── src/
│   ├── app/             # Next.js app directory
│   ├── components/      # React components
│   ├── contexts/        # React context providers
│   ├── hooks/           # Custom React hooks
│   ├── lib/             # Utilities, constants, and API logic
│   ├── providers/       # App-wide providers
│   └── types/           # TypeScript types
├── .env.example         # Example environment variables
├── drizzle.config.ts    # Drizzle ORM config
├── next.config.ts       # Next.js config
├── package.json         # Project metadata and scripts
└── README.md            # Project documentation
```

---

## Tech Stack

- **Frontend:** Next.js, React, TypeScript, Tailwind CSS
- **Smart Contracts:** Solidity (Foundry)
- **Database:** Drizzle ORM, PostgreSQL
- **Wallets:** wagmi, Coinbase OnchainKit
- **Testing:** Foundry (contracts), Jest/React Testing Library (frontend)

---

## Getting Started

### Prerequisites

- Node.js (v18+ recommended)
- pnpm (or npm/yarn)
- Foundry (for smart contract development)
- PostgreSQL (for local development)

### Installation

```bash
# Clone the repository
git clone https://github.com/benedict-drio/conclave.git
cd conclave

# Install dependencies
pnpm install

# Copy and configure environment variables
cp .env.example .env
# Edit .env with your settings

# Set up the database
pnpm db:generate
pnpm db:migrate

# Start the development server
pnpm dev
```

---

## Usage

### Running the App

1. Start the development server as above.
2. Open [http://localhost:3000](http://localhost:3000) in your browser.
3. Connect your wallet and start exploring debates!

### Environment Variables

Configure your `.env` file for API keys, database URLs, and other secrets. See `.env.example` for required variables.

---

## Smart Contracts

```bash
cd contracts
# Install Foundry if not already installed
# curl -L https://foundry.paradigm.xyz | bash

# Compile contracts
forge build

# Run tests
forge test
```

---

## Contributing

We welcome contributions! Please open issues or submit pull requests for improvements, bug fixes, or new features.

### How to Contribute

1. Fork the repository
2. Create a new branch (`git checkout -b feature/your-feature`)
3. Make your changes
4. Commit and push (`git commit -am 'Add new feature'`)
5. Open a pull request

---

## FAQ

**Q: What is Conclave?**
A: Conclave is a decentralized platform for hosting and participating in onchain debates, powered by the Base blockchain.

**Q: How do I participate in a debate?**
A: Connect your wallet, register a Basename, and join or create a debate. Stake USDC to participate and vote.

**Q: Is my data stored onchain?**
A: Core debate logic and staking are onchain. Some user data and analytics are stored offchain for performance.

**Q: How do I report bugs or request features?**
A: Please open an issue on the GitHub repository.

---

## License

This project is licensed under the MIT License.

---

## Contact

- GitHub: [benedict-drio/conclave](https://github.com/benedict-drio/conclave)
- Project Lead: [@benedict-drio](https://github.com/benedict-drio)

For questions, suggestions, or partnership inquiries, please open an issue or contact the project lead via GitHub.
