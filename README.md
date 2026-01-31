# My Dapp

A Web3 application - foundation built with Cradle

## 📁 Project Structure

```
my-dapp/
├── apps/
│   └── web/                    # Next.js frontend application
│       ├── src/
│       │   ├── app/            # App Router pages
│       │   ├── components/     # React components
│       │   │   └── contract-interactions/
│       │   │       └── ERC20InteractionPanel.tsx
│       │   └── lib/            # Utilities & wagmi config
│       ├── package.json
│       ├── tailwind.config.js
│       └── postcss.config.js
├── contracts/                  # Rust/Stylus smart contracts
│   └── erc20/                  # ERC-20 token contract source
├── docs/                       # Documentation
├── .gitignore
└── README.md
```

## 🚀 Quick Start

### Prerequisites
- Node.js 18+
- npm, yarn, or pnpm

### Installation

1. **Clone the repository:**
   ```bash
   git clone <your-repo-url>
   cd my-dapp
   ```

2. **Navigate to the web app:**
   ```bash
   cd apps/web
   ```

3. **Install dependencies:**
   ```bash
   npm install
   # or
   pnpm install
   ```

4. **Set up environment variables:**
   ```bash
   cp .env.example .env.local
   ```

   Edit `.env.local` and configure:
      - `PRIVATE_KEY`: Private key for deployment and transactions
   - `AGENT_NAME`: Name of the AI agent
   - `OPENROUTER_API_KEY`: OpenRouter API key for LLM access
   - `NEXT_PUBLIC_AGENT_NETWORK`: Network for agent operations (arbitrum or arbitrum-sepolia)

   > **Get a WalletConnect Project ID** at [WalletConnect Cloud](https://cloud.walletconnect.com/)

5. **Start the development server:**
   ```bash
   npm run dev
   ```

6. **Open your browser:**
   Visit [http://localhost:3000](http://localhost:3000)

## 🔗 Smart Contracts

The `contracts/` folder contains Rust/Stylus smart contract source code.

**Default deployed contracts (Arbitrum Sepolia testnet):**
- ERC-20: `0x5af02ab1d47cc700c1ec4578618df15b8c9c565e`

## 🛠 Available Scripts

Run these from the `apps/web` directory:

| Command | Description |
|---------|-------------|
| `npm run dev` | Start development server |
| `npm run build` | Build for production |
| `npm run start` | Start production server |
| `npm run lint` | Run ESLint |

## 🌐 Supported Networks

- Arbitrum Sepolia (Testnet)
- Arbitrum One (Mainnet)
- Superposition
- Superposition Testnet

## 📚 Tech Stack

- **Framework:** Next.js 14 (App Router)
- **Styling:** Tailwind CSS
- **Web3:** wagmi + viem
- **Wallet Connection:** RainbowKit

## 📖 Documentation

See the `docs/` folder for:
- Contract interaction guide
- Deployment instructions
- API reference

## License

MIT

---

Generated with ❤️ by [Cradle](https://cradle.dev)
