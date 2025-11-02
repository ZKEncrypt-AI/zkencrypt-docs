---
layout: home

hero:
  name: ZKEncrypt Network
  text: Privacy-Preserving AI Infrastructure
  tagline: Build confidential dApps with Fully Homomorphic Encryption on Solana
  actions:
    - theme: brand
      text: Get Started
      link: /guide/getting-started
    - theme: alt
      text: View on GitHub
      link: https://github.com/ZKEncrypt-AI

features:
  - icon: 🔐
    title: Fully Homomorphic Encryption
    details: Compute on encrypted data without decryption. Keep sensitive information private while enabling powerful on-chain operations.
  
  - icon: ⚡
    title: High Performance
    details: Built on Solana for 50k+ TPS. x402 micropayments enable sub-cent transactions for AI inference and privacy operations.
  
  - icon: 🤖
    title: AI Oracle Integration
    details: Query AI models with encrypted prompts. Privacy-preserving machine learning for decentralized applications.
  
  - icon: 🔄
    title: Private DeFi
    details: Hidden balances, confidential swaps, and sealed-bid auctions. Build the next generation of privacy-first financial applications.
  
  - icon: 🛠️
    title: Developer Friendly
    details: Solidity-compatible smart contracts, TypeScript SDK, and comprehensive CLI tools. Start building in minutes.
  
  - icon: 🌐
    title: Cross-Chain Ready
    details: Interoperable privacy layer for Ethereum, Solana, and beyond. Bridge encrypted data across multiple networks.
---

## Quick Start

Install the SDK and start building:

```bash
npm install @zkencrypt/sdk
```

```typescript
import { ZKEncryptSDK } from '@zkencrypt/sdk';

const sdk = new ZKEncryptSDK({
  network: 'mainnet-beta',
});

// Encrypt data
const encrypted = await sdk.encrypt({
  data: 'Sensitive information',
  publicKey: userPublicKey,
});

// Send private payment
const payment = await sdk.sendPayment({
  recipient: 'RECIPIENT_ADDRESS',
  amount: 0.001,
  encrypted: true,
});
```

## Why ZKEncrypt?

### True Privacy
Unlike zero-knowledge proofs that only verify computations, FHE keeps data encrypted throughout the entire process. Your sensitive information never leaves encryption.

### Production Ready
Battle-tested infrastructure with enterprise-grade security. Used by leading DeFi protocols and privacy-focused applications.

### Open Source
Fully open-source libraries and tools. Join our community of developers building the future of private computing.

## Ecosystem

- **[SDK](https://github.com/ZKEncrypt-AI/zkencrypt-sdk)** - JavaScript/TypeScript library
- **[Solidity](https://github.com/ZKEncrypt-AI/zkencrypt-solidity)** - Smart contract library
- **[CLI](https://github.com/ZKEncrypt-AI/zkencrypt-cli)** - Command-line tools
- **[Examples](https://github.com/ZKEncrypt-AI/zkencrypt-examples)** - Sample applications
- **[Docs](https://github.com/ZKEncrypt-AI/zkencrypt-docs)** - This documentation

## Community

- [Twitter](https://x.com/ZKEncrypt_AI)
- [GitHub](https://github.com/ZKEncrypt-AI)
- [Gitbook](https://zkencrypt-ai.gitbook.io/zkencrypt-ai)
