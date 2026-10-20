# QuantumPools

**Multi-chain concentrated-liquidity management and analytics** — Uniswap, PancakeSwap, Aerodrome, Orca, Meteora, and Solana, with Cover Value–style reporting, snuggle, and ETH hedging workflows.

## Main site (canonical app)

**https://app.quantumpools.io** is the primary QuantumPools product URL. Use this exact URL in wallet, directory, and DefiLlama-style listings.

https://quantumpools.io is the marketing / metrics host (not the main app).

## Supported chains

Self-withdrawable managed vaults are deployed on:

- Robinhood Chain
- Base
- BNB Smart Chain (BSC)

BNB Smart Chain (BSC) is the EVM network of BNB Chain (chain id 56).

| Chain | Vault |
| --- | --- |
| BNB Smart Chain (BSC) / BNB Chain | `0x9597f68203d1bc85744A5Fc11D890aA7777e386B` |

On BNB Smart Chain (BSC), `0x9597f68203d1bc85744A5Fc11D890aA7777e386B` is the QuantumPools self-withdrawable managed vault. The depositor stays the recorded owner and can withdraw. When a position leaves its range, automatic snuggle moves the range. Owner controls are timelocked, and the performance fee is hard-capped and charged on trading fees only — never on principal.

## What it is

QuantumPools is a multi-chain concentrated-liquidity manager and analytics platform. It covers Uniswap, PancakeSwap, Aerodrome, Orca, Meteora, and Solana venues on Robinhood Chain, Base, and BNB Smart Chain (BSC), with per-position LP bookkeeping, Cover Value–style deposit-versus-hold reporting, multi-sleeve range strategies, owner-tunable snuggle timing, and ETH hedging workflows.

On these EVM deployments, LP NFTs can sit in a QuantumPools self-withdrawable managed vault. Automatic snuggle is the range adjustment. Withdrawal stays available to the position owner, owner controls are timelocked, and the performance fee is hard-capped and charged on trading fees only — never on principal.

Available analytics, indexing, vault management, and hedging features vary by venue and network. Listing a venue or chain here does not mean every feature ships on every chain yet.

## Official links and contact

- **Main app:** [app.quantumpools.io](https://app.quantumpools.io)
- Marketing / metrics: [quantumpools.io](https://quantumpools.io)
- Metrics page: [quantumpools.io/metrics.html](https://quantumpools.io/metrics.html)
- X: [@QuantumPoolsIO](https://x.com/QuantumPoolsIO)
- Contact: admin@quantumpools.io
- Public identity and brand assets: this repository

## Wallet and directory review

- [General listing packet](docs/WALLET-LISTING.md)
- [Rabby review packet and source-traced warning diagnosis](docs/RABBY-REVIEW.md)
- [Structured project identity (JSON-LD)](identity.json)

These are project-published information resources, not independent approval. The JSON-LD is generic project metadata, not a universal wallet allowlist file. Submitting a packet does not mean a wallet has approved or listed the app.

## Logos

- [250 px PNG](assets/dappradar-logo-250.png)
- [400 px PNG](assets/logo-400.png)
- [400 px JPG](assets/logo-400.jpg)

## Source-code privacy and verification

Source for the production application is maintained privately. This repository contains public project information and brand assets, not the proprietary application, backend, keeper logic, Cover Value implementation, snuggle internals, or credentials.

A project listing or wallet recognition is not a security audit or a guarantee of investment performance. Audit links may be added later; this packet intentionally omits them for now. QuantumPools does not claim ownership of third-party protocols' contracts or their total value locked merely because it tracks or interacts with them.

Always verify the app domain (**app.quantumpools.io**) and review wallet permissions and transaction details before signing. Never provide a seed phrase or private key to a website or support contact.

---

© QuantumPools · Not financial advice.
