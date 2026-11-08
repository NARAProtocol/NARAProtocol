# NARA Protocol V5 & CryptoSLIP V3.2 — Base Mainnet (`Chain ID: 8453`)

[![Website](https://img.shields.io/badge/Website-naraprotocol.io-00FF9D?style=flat-square&logo=google-chrome&logoColor=black)](https://naraprotocol.io)
[![Launch CryptoSLIP](https://img.shields.io/badge/Launch_App-CryptoSLIP_V3.2-00E5FF?style=flat-square&logo=ethereum&logoColor=black)](https://cryptoslip-g29s.4everland.app/?v=cs-1794113891779)
[![Public Docs & Audit Verification](https://img.shields.io/badge/Docs_&_Verification-nara__protocol-3B82F6?style=flat-square&logo=github&logoColor=white)](https://github.com/NARAProtocol/nara_protocol)
[![Base Mainnet](https://img.shields.io/badge/Network-Base_Mainnet_(8453)-0052FF?style=flat-square&logo=coinbase&logoColor=white)](https://basescan.org/token/0x91FB78A9F46B67f54BbD4489941d19666b2fAe0f)
[![X (Twitter)](https://img.shields.io/badge/X-@NARA__protocol-000000?style=flat-square&logo=x&logoColor=white)](https://x.com/NARA_protocol)
[![Telegram](https://img.shields.io/badge/Telegram-@NARAProtocol-26A5E4?style=flat-square&logo=telegram&logoColor=white)](https://t.me/NARAProtocol)
[![AI / LLM Ready](https://img.shields.io/badge/AI_&_LLM_Index-llms.txt_%7C_llms--full.txt-10B981?style=flat-square)](https://github.com/NARAProtocol/nara_protocol/blob/main/llms-full.txt)

**NARA Protocol V5** is an autonomous, non-custodial on-chain value commitment and multi-asset reward distribution protocol deployed on **Base Mainnet (`Chain ID: 8453`)**, paired natively with **CryptoSLIP V3.2**—a gasless, 1:1 isolated bearer-voucher (`Slip`) and in-vault DEX settlement layer.

- **Fixed Supply & Sealed Reserve:** `1,000,000 NARA` hard cap (`0%` ERC-20 transfer tax, EIP-2612 `Permit`, no `mint()` capability). `949,987 NARA` (`94.9987%`) is permanently sealed inside [`NARAEmissionReserveV5`](https://basescan.org/address/0xf932178F24b0813C82093985F0Af6Db27Ae25930#code) (`_bootstrapAuthority == 0x0`, `_bindingsSealed == true`) over a 4-year horizon (`140,160` fifteen-minute pulses).
- **Physical Principal / Reward Segregation:** Committed user principal (`1.0 NARA` minimum per 1:1 ERC-721 `NARAP` Position NFT; no NFT splitting or fusion) sits inside [`NARAPrincipalLedgerV5`](https://basescan.org/address/0x7F866a9fbe41D54F0d9C35b6892fcf27Ea766DB2#code) (no lending, flash-loan, or admin sweep capability), physically isolated from 15-minute (`900-second`) multi-asset rewards (`NARA`, `ETH`, `USDC`) in [`NARARewardLedgerV5`](https://basescan.org/address/0xC72671D9438388638547444524F6542b650C9264#code).
- **CryptoSLIP V3.2 (`Commit NARA` & Gasless Bearer Vouchers from `0.001 NARA`):** Commit `1.0+ NARA` (`1–365 days`), harvest 15-minute rewards into shareable links, or send, split, combine, and swap `USDC`, `cbBTC`, `ETH`, and `NARA` (`>= 0.001 NARA`) via shareable links, QR codes, or 69-byte off-grid LoRa radio packets without requiring `ETH` for gas or exposing personal wallet balances on BaseScan.

---

## Choose Your Path (4-Persona Navigation Router)

| Audience | Recommended Entry Point | Key Resources |
|---|---|---|
| **1. Everyday Users & Newcomers** | [**Launch CryptoSLIP V3.2 App**](https://cryptoslip-g29s.4everland.app/?v=cs-1794113891779) | • [**User Guide (`User_Guide.md`)**](https://github.com/NARAProtocol/nara_protocol/blob/main/docs/User_Guide.md)<br>• [**Dispatch #00: Genesis Introduction**](https://github.com/NARAProtocol/nara-v5-dispatches/blob/main/dispatches/00-GENESIS-INTRODUCTION.md)<br>• [**Interactive Portal (`naraprotocol.io`)**](https://naraprotocol.io) |
| **2. DeFi Integrators & Protocol Developers** | [**Technical Architecture (`Technical_Architecture.md`)**](https://github.com/NARAProtocol/nara_protocol/blob/main/docs/Technical_Architecture.md) | • [**Core Contract Stack (`nara_protocol_v4`)**](https://github.com/NARAProtocol/nara_protocol_v4)<br>• [**Machine-Readable Manifest (`deployment.json`)**](https://github.com/NARAProtocol/nara_protocol/blob/main/verification/deployment.json)<br>• [**Category Baskets (`nara_protocol_v4_baskets`)**](https://github.com/NARAProtocol/nara_protocol_v4_baskets) & [**Swarm Monitor**](https://github.com/NARAProtocol/nara-swarm-monitor) |
| **3. Security Auditors, Legal & Compliance Reviewers** | [**Verification & Audit Hub (`verification/README.md`)**](https://github.com/NARAProtocol/nara_protocol/blob/main/verification/README.md) | • [**Investor & Auditor Due-Diligence Q&A (`NARA_INVESTOR_QNA.md`)**](https://github.com/NARAProtocol/nara_protocol/blob/main/docs/NARA_INVESTOR_QNA.md)<br>• [**58M+ Fuzz & Formal Invariant Dispatch (`#06`)**](https://github.com/NARAProtocol/nara-v5-dispatches/blob/main/dispatches/06-THE-VOLVO-CRANE-DROP-58M-FUZZ-TESTS.md)<br>• [**Security & Disclosure Policy (`SECURITY.md`)**](https://github.com/NARAProtocol/nara_protocol/blob/main/SECURITY.md) |
| **4. AI Assistants, LLMs & RAG Crawlers** | [**Complete AI Context (`llms-full.txt`)**](https://github.com/NARAProtocol/nara_protocol/blob/main/llms-full.txt) | • [**Compact LLM Index (`llms.txt`)**](https://github.com/NARAProtocol/nara_protocol/blob/main/llms.txt)<br>• [**Project Knowledge Base (`PROJECT_KNOWLEDGE_BASE.md`)**](https://github.com/NARAProtocol/nara_protocol/blob/main/docs/PROJECT_KNOWLEDGE_BASE.md)<br>• [**Architectural Dispatches (`nara-v5-dispatches`)**](https://github.com/NARAProtocol/nara-v5-dispatches) |

---

## Official Repository Directory

| Repository | Scope & Purpose | Verification / Status |
|---|---|---|
| [**`NARAProtocol/nara_protocol`**](https://github.com/NARAProtocol/nara_protocol) | **Canonical Public Documentation, Audit Verification Suite & AI Knowledge Base.** Contains all architecture specifications, investor/auditor Q&A, `llms-full.txt`, and the zero-dependency Base RPC verification suite (`npm run verify:onchain`). | `35 / 35` V5 contracts verified on Base (`8453`) |
| [**`NARAProtocol/nara_protocol_v4`**](https://github.com/NARAProtocol/nara_protocol_v4) | **Core Smart-Contract Engineering & Formal Verification Stack.** Houses the NARA V5 core contracts, Uniswap v4 liquidity hook, deployment manifests, and invariant test suites. | Production Base Mainnet (`8453`) |
| [**`NARAProtocol/nara-v5-dispatches`**](https://github.com/NARAProtocol/nara-v5-dispatches) | **Curated Architectural Dispatches & AI RAG Knowledge Base.** Deep-dive technical articles covering the 949,987 NARA sealed reserve, 1:1 isolated Slips, 3-tier UTXO `slipId` provenance, gasless EIP-712 permits, 69-byte LoRa radio Slips, and 58M+ fuzz tests. | Dispatches `#00`–`#07` + Formal Specs |
| [**`NARAProtocol/nara-swarm-monitor`**](https://github.com/NARAProtocol/nara-swarm-monitor) | **Read-Only Operations Intelligence & Invariant Telemetry.** Real-time on-chain indexer and health monitor tracking epoch settlements, reserve accounting, and pool telemetry on Base. | Read-only telemetry (`8453`) |
| [**`NARAProtocol/nara_protocol_v4_baskets`**](https://github.com/NARAProtocol/nara_protocol_v4_baskets) | **Non-Custodial Receipt-Based Category Baskets (`CORE`, `AI`, `FINANCE`, `CULTURE`).** Immutable pro-rata multi-token basket contracts and preview interface on Base (`0x43072323dB49c36ab3725b07DF3bf02c4176f89C`). | Deployed & Verified on Base (`8453`) |
| [**`NARAProtocol/nara-landing`**](https://github.com/NARAProtocol/nara-landing) | **Official Web Portal (`naraprotocol.io`).** Static Vite + Cloudflare Pages portal with strict CSP, security headers, and AI discovery endpoints. | Live at [`naraprotocol.io`](https://naraprotocol.io) |

---

## Canonical Base Mainnet (`Chain ID: 8453`) Contracts

All 35 NARA V5 contracts and all CryptoSLIP V3.2 contracts are deployed and source-verified on BaseScan. Full 35-contract manifest: [`verification/deployment.json`](https://github.com/NARAProtocol/nara_protocol/blob/main/verification/deployment.json).

### NARA Protocol V5 Core & Liquidity Stack

| Contract | Address (Base `8453`) | Role & Architectural Invariant |
|---|---|---|
| **`NARATokenV5`** | [`0x91FB78A9F46B67f54BbD4489941d19666b2fAe0f`](https://basescan.org/token/0x91FB78A9F46B67f54BbD4489941d19666b2fAe0f) | Canonical `NARA` ERC-20 (`1,000,000` fixed supply, `18` decimals, `0%` transfer tax, EIP-2612 `Permit`) |
| **`NARAEmissionReserveV5`** | [`0xf932178F24b0813C82093985F0Af6Db27Ae25930`](https://basescan.org/address/0xf932178F24b0813C82093985F0Af6Db27Ae25930#code) | Sealed `949,987 NARA` emission reserve (`140,160` pulses / 4-year horizon, `_bootstrapAuthority = 0x0`) |
| **`NARAEpochEngineV5`** | [`0xd93FbEbFb33FAc9288125074625D4750573B1a53`](https://basescan.org/address/0xd93FbEbFb33FAc9288125074625D4750573B1a53#code) | Autonomous `900-second` (15-minute) epoch settlement & reserve release coordinator |
| **`NARAPrincipalLedgerV5`** | [`0x7F866a9fbe41D54F0d9C35b6892fcf27Ea766DB2`](https://basescan.org/address/0x7F866a9fbe41D54F0d9C35b6892fcf27Ea766DB2#code) | Segregated 1:1 user principal vault (`1.0 NARA` minimum per NFT; zero lending, flash-loan, or admin sweep capability) |
| **`NARARewardLedgerV5`** | [`0xC72671D9438388638547444524F6542b650C9264`](https://basescan.org/address/0xC72671D9438388638547444524F6542b650C9264#code) | Multi-asset (`NARA`, `ETH`, `USDC`) reward ledger (`80%` Base / `20%` Rarity split at `1e27` precision) |
| **`NARAPositionNFTV5`** | [`0x8C5F088D9d09dBB90aB6F3aaA049a8FD5D5FfFDA`](https://basescan.org/address/0x8C5F088D9d09dBB90aB6F3aaA049a8FD5D5FfFDA#code) | ERC-721 commitment position receipt with on-chain SVG metadata |
| **`NARAPositionSaleV5`** | [`0x04Ac83045d26259D46400Ce6beb9bBd0641df225`](https://basescan.org/address/0x04Ac83045d26259D46400Ce6beb9bBd0641df225#code) | Atomic secondary escrow marketplace with `_checkAcquisition` `BuyerBounds` front-run protection |
| **`NARALiquidityHookV5`** | [`0x07d8F2Dfd121B10dE3176DeAb6A8C0eaa2646aCC`](https://basescan.org/address/0x07d8F2Dfd121B10dE3176DeAb6A8C0eaa2646aCC#code) | Uniswap v4 Hook (`USDC/NARA` pool `0x4a475299ef674bcc3d2c87c3917cfbecd38cf7237646a3553e37daba67da6e5f`) |
| **`NARAFeeVaultV5`** | [`0xF1f361F803895BF5cf67eC6C506dbFEf2f6E88Cf`](https://basescan.org/address/0xF1f361F803895BF5cf67eC6C506dbFEf2f6E88Cf#code) | Hook fee vault sealed to zero-delay `NARATreasuryFeeControllerV5` (`0xB6A436b48222C94fe427ecAfB263DF9cf42646b9`) and `NARAFeeIngressBindingV5` (`0x17cc74317AD75a170887F9E76e5fF09f2058d4BF`) |
| **`NARATreasuryRangeManagerV5`** | [`0x221c625d2BC416460C397035C1286C1f4A4D3A7C`](https://basescan.org/address/0x221c625d2BC416460C397035C1286C1f4A4D3A7C#code) | Active rule-bound Uniswap v4 CLAMM range manager (Legacy: `0xa72557fcBE56B3eC739dF3aF7b6b893B6Db4D288`) |

### CryptoSLIP V3.2 Core Stack

| Contract | Address (Base `8453`) | Role & Architectural Invariant |
|---|---|---|
| **`CryptoSlipVaultV32`** | [`0x38BF0321FA7489576978353a6a8da4A3e85C2F18`](https://basescan.org/address/0x38BF0321FA7489576978353a6a8da4A3e85C2F18#code) | Non-custodial 1:1 isolated bearer-voucher vault (`USDC`, `cbBTC`, `ETH`, `NARA`) with UTXO `slipId` provenance |
| **`CryptoSlipNFTV32`** | [`0x36181Ca1B0210b6Ea8E56755dA7B06c34ba481C0`](https://basescan.org/address/0x36181Ca1B0210b6Ea8E56755dA7B06c34ba481C0#code) | ERC-721 + EIP-2981 transferable voucher receipt |
| **`CryptoSlipTradeRouterV32`** | [`0x295E72cB3dc09582F32e0fEB7e0e650752219a7f`](https://basescan.org/address/0x295E72cB3dc09582F32e0fEB7e0e650752219a7f#code) | Atomic in-vault Slip-to-Slip DEX swap, limit order, and P2P barter router |

---

## Independent 1-Command On-Chain Verification

Anyone can independently verify the live Base Mainnet (`8453`) deployment, runtime bytecode hashes, immutable cross-module bindings, and sealed `949,987 NARA` emission reserve directly against Base RPC with zero third-party dependencies:

```bash
git clone https://github.com/NARAProtocol/nara_protocol.git
cd nara_protocol
npm ci
npm run verify
npm run verify:onchain
```
