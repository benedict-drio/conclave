# Conclave

Conclave is a decentralized debate platform built on Base, empowering users to stake USDC, engage in meaningful debates, and let the community decide the outcome. Designed for transparency, fairness, and onchain reputation, Conclave brings the spirit of open discourse to the web3 era.

## Features

- **Decentralized Debates:** Create, join, and participate in debates with real stakes.
- **Onchain Identity:** Use Basename for unique, verifiable onchain identities.
- **Staking Mechanism:** Stake USDC to participate and show conviction.
- **Community Voting:** Let the community determine the winning arguments.
- **Leaderboard & Reputation:** Track top debaters and build your onchain reputation.
- **Smart Wallet Integration:** Seamless wallet connection for secure transactions.

## Tech Stack

- **Frontend:** Next.js, React, TypeScript, Tailwind CSS
- **Smart Contracts:** Solidity (Foundry)
- **Database:** Drizzle ORM, PostgreSQL
- **Wallets:** wagmi, Coinbase OnchainKit

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

### Smart Contracts
```bash
cd contracts
# Install Foundry if not already installed
# curl -L https://foundry.paradigm.xyz | bash
# Compile contracts
 forge build
# Run tests
 forge test
```

## Contributing
We welcome contributions! Please open issues or submit pull requests for improvements, bug fixes, or new features.

## License
This project is licensed under the MIT License.

## Acknowledgments
- Built with Next.js, Foundry, and the Base ecosystem
- Inspired by the spirit of open, onchain discourse
