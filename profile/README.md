# BeanChain

**BeanChain** is a modular, transparent blockchain ecosystem built for speed, flexibility, and developer empowerment. Designed with a layered architecture, extensible transaction system, and a strong focus on customizability, BeanChain supports both on-chain and off-chain logic, multi-language contract execution, and permissionless node development.

> Currently in devnet phase — powered by a growing set of core tools, core nodes, and custom SDKs maintained by the **BeanChain Core Team** under **Outlandish Tech**, a division of **Outlandish Creative LLC**.

---

## Core Architecture

At the heart of BeanChain is a flexible, layered node system that allows the network to scale horizontally and vertically:

- **GPN – Genesis Public Node**  
  The first public node on the chain. Acts as the anchor for synchronization and transaction gossip.

- **PN – Public Node**  
  Public-facing node for wallet access and transaction relay. Maintains Spring Boot APIs for integration.

- **RN – Reward Node**  
  Handles system-level transaction generation: faucet payouts, validator gas rewards, early wallet distributions. Also tracks validator trust scores via ping/pong logic.  
  [GitHub Repo → BeanChain-Core/RN](https://github.com/BeanChain-Core/RN)

- **CEN – Contract Execution Node**  
  Executes off-chain smart contract logic and initiates contract-based Layer 1 or Layer 2 transactions.

- **Historical Node** *(Coming Soon)*  
  A SQL-powered node that stores block history and exposes high-performance, load-balanced endpoints for explorers and DApps.

> Peripheral nodes like the CEN and Historical Node will be released in **barebones, customizable form**, allowing developers to build and extend node logic freely while connected to the network.

---

## Technology Highlights

- **Custom Transaction Types & Flags**  
  Built-in support for `transfer`, `reward`, `airdrop`, `mint`, `contractCall`, `fundedCENCALL`, and more.

- **Off-Chain Contract Execution**  
  Via CENs, enabling lightweight contract logic without bloating consensus layers.

- **Layer 2 Token Framework**  
  Full minting, burning, and transferring support for fungible tokens, stored and indexed in the Layer2DB.

- **Peripheral Node Flexibility**  
  Build custom nodes that connect to the network and trigger logic — including oracles, APIs, automation, and more.

- **Multi-Language Contract Support** *(in progress)*  
  Java support is live. Go, Python, and JS support are in planning to open the CEN to any developer language.

- **Shared Core SDK**  
  [`BeanPack-Java`](https://github.com/BeanChain-Core/BeanPack-Java) — the official Java SDK providing transaction logic, hashing, Merkle tree utilities, and model definitions for Java-based tools and nodes.

---

## Ecosystem Projects

| Project | Description |
|--------|-------------|
| [`BeanNode`](https://github.com/BeanChain-Core/BeanNode) | Main validator node implementation (GPN, PN, PRN) |
| [`BeanPack-Java`](https://github.com/BeanChain-Core/BeanPack-Java) | Shared SDK for transactions, signatures, and node logic |
| [`LimaBeanWallet`](https://github.com/BeanChain-Core/LimaBeanWallet) | Wallet frontend for sending transactions, minting tokens, and managing assets |
| [`BeanChain.io`](https://github.com/BeanChain-Core/BeanChain.io) | Visual block explorer and documentation hub |
| [`Reward Node (RN)`](https://github.com/BeanChain-Core/RN) | System-level transaction engine for rewards and faucets |
| *Contract Execution Node (CEN)* | Contract processor — **repo coming soon** |
| *Historical Node* | SQL-based block fetch node — **repo coming soon** |
| *BaseNode* | Lightweight network-ready shell for oracles and custom tools — **repo coming soon** |

---

## What’s Coming

- **Discord Community Launch**  
  Full public server for devs, builders, validators, and explorers

- **Historical Node Deployment**  
  Clustered, load-balanced fetch system for explorers and DApps

- **GhostNet Testnet**  
  A themed public fork of the chain for creative, chaotic testing

- **Lightweight Node Kits**  
  Portable skeletons for oracles, bots, games, and network-connected tools

---

## Get Involved

BeanChain is still in early development — but growing fast. We’re looking for open-source contributors, blockchain engineers, infrastructure builders, and curious tinkerers to join the next wave of decentralized tooling.

📬 **Reach out:** `team@limabean.xyz`

---

Crafted by the **BeanChain Core Team**  
Under **Outlandish Tech**, powered by **Outlandish Creative LLC**
