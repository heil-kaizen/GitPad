# Solana Pump-Style Launchpad (MVP)

A **minimal Pump.fun-style token launchpad** built on **Solana Devnet**.  
This project is an **MVP demo** created for learning, experimentation, and showcasing — **not production**.

Users can create tokens and **buy/sell instantly** using a **bonding curve AMM**, with no external liquidity pools.

---

## 🚨 Disclaimer (Read This First)

This project is:

- 🚧 **Experimental**
- 🧪 **Unaudited**
- 🧠 **For learning & demos only**
- ❌ **Not production-ready**
- ❌ **Not financial advice**

Use at your own risk. Funds on Devnet only.

---

## ✨ Features

- 🪙 **Create SPL tokens** instantly
- ⚡ **Buy & sell immediately** after creation
- 📈 **Bonding curve AMM** (Pump.fun-style)
- 🔥 Tokens are **minted on buy**, **burned on sell**
- 🔐 **Mint & freeze authority revoked** on creation
- 🧑‍💻 Dev can buy/sell instantly (no locks)
- 👥 Anyone can trade any token
- 🌐 **Fully public frontend**
- 🧱 **No backend, no database**
- 🔍 Tokens fetched **directly from on-chain accounts**

---

## 🧠 How It Works (High Level)

- Tokens are created via an **Anchor smart contract**
- A **virtual liquidity bonding curve** determines price
- SOL is stored in a program vault
- Tokens are minted when users buy
- Tokens are burned when users sell
- Market cap is derived from:
  




No Raydium. No external pools. No middlemen.

---

## 🏗 Tech Stack

### Blockchain
- **Solana Devnet**
- **Anchor (Rust)**
- **SPL Token**
- **Phantom Wallet**

### Frontend
- **Next.js**
- **TypeScript**
- **Tailwind CSS**
- **Solana Wallet Adapter**

### Hosting
- **Replit (public URL)**

---

## 🗂 Project Structure

```text
.
├── Anchor.toml
├── Cargo.toml
├── programs/
│   └── launchpad/
│       ├── src/
│       │   └── lib.rs
│       └── Cargo.toml
├── app/
│   ├── page.tsx          # Trenches (Landing page)
│   ├── create/page.tsx  # Create token
│   └── token/[mint]/    # Token detail (buy/sell)
├── public/
├── README.md
└── package.json
