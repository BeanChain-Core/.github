# BeanChain

**BeanChain** is a modular, transparent blockchain ecosystem built for speed, flexibility, and developer empowerment. With a layered architecture, extensible transaction system, and a strong focus on permissionless node development, BeanChain supports both on-chain and off-chain logic, multi-language contract execution, and open tooling for infrastructure builders.

> Currently in devnet phase — powered by a growing set of core tools, node frameworks, and SDKs maintained by the **BeanChain Core Team** under **Outlandish Tech**, a division of **Outlandish Creative LLC**.

---

## Core Architecture

At the heart of BeanChain is a flexible, layered node system designed to scale horizontally and vertically:

- **GPN – Genesis Public Node**  
  The first public node on the chain. Acts as the bootstrap anchor for synchronization and transaction gossip.

- **PN – Public Node**  
  Public-facing node for wallets and dApps. Maintains REST endpoints for sending and syncing transactions.

- **RN – Reward Node**  
  Handles system-level transaction generation, including faucet payouts, validator rewards, and early wallet distributions. Also tracks validator trust scores through ping/pong logic.  
  → [GitHub Repo – BeanChain-Core/RN](https://github.com/BeanChain-Core/RN)

- **CEN – Contract Execution Node** *(in development)*  
  Executes off-chain smart contract logic and triggers Layer 1 or Layer 2 transactions. Contracts like staking will launch here first.

- **Historical Node** *(in development)*  
  A SQL-powered node that archives blocks and exposes high-throughput, load-balanced endpoints for explorers and external apps.

> Peripheral nodes like the CEN and Historical Node will be released in **barebones, customizable form**, allowing developers to plug in their own contract logic, data services, or analytics layers using real-time sync from open Public Nodes.

---

## Technology Highlights

- **Custom Transaction Types & Flags**  
  Built-in support for `transfer`, `reward`, `airdrop`, `mint`, `contractCall`, `fundedCENCALL`, and more.

- **Off-Chain Contract Execution**  
  Through CENs, enabling scalable contract logic without bloating consensus layers.

- **Layer 2 Token Framework**  
  Mint, burn, and transfer custom tokens. All tokens are tracked in the Layer2DB, separate from the core state tree.

- **Peripheral Node Flexibility**  
  Build your own nodes that connect to the network and trigger custom logic — including oracles, event-driven bots, and data relays.

- **Multi-Language Contract Support** *(in progress)*  
  Java support is live. Go, Python, and JavaScript support is planned for broader accessibility via the CEN.

- **Shared Core SDK**  
  [`BeanPack-Java`](https://github.com/BeanChain-Core/BeanPack-Java) — the official SDK used across all Java-based nodes, containing shared models, crypto tools, and core transaction logic.

---

## Ecosystem Projects

**All projects are in active development.**

| Project | Description |
|--------|-------------|
| [`BeanNode`](https://github.com/BeanChain-Core/BeanNode) | Core validator node for GPN, PN, and PRN roles |
| [`BeanPack-Java`](https://github.com/BeanChain-Core/BeanPack-Java) | Shared Java SDK powering all core node logic |
| [`LimaBeanWallet`](https://github.com/BeanChain-Core/LimaBeanWallet) | Wallet interface for managing BEAN and tokens |
| [`BeanChain.io`](https://github.com/BeanChain-Core/BeanChain.io) | Official network hub — explorer and staking portal launching soon |
| [`Reward Node (RN)`](https://github.com/BeanChain-Core/RN) | System transaction generator and reward distributor |
| *Contract Execution Node (CEN)* | Off-chain contract logic executor — **repo coming soon** |
| *Historical Node* | SQL block storage + fetch API layer — **repo coming soon** |
| [`BaseNode (xNodeTemplate)`](https://github.com/BeanChain-Core/BaseNode) | Lightweight skeleton for oracles, bots, and custom node logic |

---

## What's Coming

- **Discord Community Launch**  
  Our public server for devs, validators, builders, and explorers

- **Historical Node Framework**  
  Kubernetes-powered block fetch system for DApps and explorers

- **GhostNet Testnet**  
  A themed, public fork of BeanChain for experimental deployments and open chaos testing

- **Lightweight Node Kits**  
  Customizable base node templates for external tools, games, and data agents

---

## Get Involved

BeanChain is still early — but growing fast. We’re building in the open and welcoming new contributors.

**Technical Contributors:**
- Core protocol developers
- Smart contract authors
- Infrastructure engineers
- Open-source contributors

**Creative & Community Roles:**
- Digital artists and asset designers  
- UI/UX and product designers  
- Discord moderators and community builders  
- Explorers, testers, and curious minds  

If you're excited by decentralized infrastructure, experimental tech, and collaborative creativity — there's a place for you here.

📬 **Contact us:** `team@limabean.xyz`  
💬 **Join the community:** [discord.gg/RMgbSkNF](https://discord.gg/RMgbSkNF)

---

Crafted by the **BeanChain Core Team**  
Under **Outlandish Tech**, powered by **Outlandish Creative LLC**

