# Getting Started with Arqma Wallet

Arqma Wallet is the official, non-custodial wallet for the Arqma (ARQ) privacy network. If you're setting it up for the first time, the process is short, but a few steps matter more than they look — especially the one where your wallet shows you a 25-word phrase and never shows it again.

This guide walks through the decisions you'll make in your first ten minutes with the wallet, and points to the deeper guides for each step.

## 1. Pick a build

Arqma Wallet ships in three forms, and picking the right one up front saves you from switching later:

- **GUI desktop wallet** — an Electron app for Windows, macOS, and Linux. This is what most people should start with. It can run a full local node or connect to a remote one.
- **CLI wallet** — command-line binaries for advanced users and server operators who want scripting and minimal overhead.
- **Mobile wallet** — native iOS and Android apps that operate as light, remote-node clients by default.

The full breakdown of tradeoffs between these three — sync time, control, and where your keys actually live — is covered in [Arqma Wallet types compared](https://arqmawallet.com/guides/wallet-types). If you're wondering whether the browser-based web wallet is a safe option too, read [Is the Arqma web wallet safe?](https://arqmawallet.com/guides/web-wallet) before you use it for anything beyond testing.

## 2. Download from the official source

Downloads are published at [arqmawallet.com/download](https://arqmawallet.com/download). Because Arqma Wallet is open-source and unaffiliated with any single company, there's no app-store gatekeeper double-checking the publisher for you on desktop — so the download page and the GitHub release page are the two sources you should trust, nothing else.

Platform-specific installation steps, including what to do about unsigned-binary warnings from Windows SmartScreen or macOS Gatekeeper, are covered per platform:

- [Install on Windows](https://arqmawallet.com/guides/install-windows)
- [Install on macOS](https://arqmawallet.com/guides/install-macos)
- [Install on Linux](https://arqmawallet.com/guides/install-linux)
- [Mobile setup for iPhone and Android](https://arqmawallet.com/guides/mobile-setup)

## 3. Create your wallet

On first launch, the wallet generates a new keypair locally on your device and shows you a **25-word seed phrase**. This is the single most important moment in the setup process. That phrase is the only backup of your funds that will ever exist — not your password, not the app, not any account, because there is no account. Anyone who has read [How non-custodial Arqma Wallet works](https://arqmawallet.com/how-it-works/non-custodial) will recognize the pattern: the wallet trades a support line for full user control, and the seed phrase is the price of that control.

Write the phrase down before you do anything else. Don't screenshot it, don't paste it into a notes app, and don't move on to funding the wallet until it's physically recorded somewhere durable. The full standard is in [Arqma seed phrase security](https://arqmawallet.com/security/seed-phrase), and the mistakes people actually make with backups — not hypothetical ones — are catalogued in [Seven backup mistakes that drain wallets](https://arqmawallet.com/security/backup-mistakes).

## 4. Choose local node or remote node

Your desktop wallet can either run its own copy of the Arqma blockchain (a local node) or connect to someone else's public node (a remote node). Local gives you the strongest privacy guarantee, since no third party sees which addresses you're checking. Remote is faster to set up and lighter on disk space, at the cost of that node operator seeing your wallet's activity pattern.

[What is an Arqma node?](https://arqmawallet.com/how-it-works/nodes) explains the difference in plain terms, and [Set up a remote node in Arqma Wallet](https://arqmawallet.com/recovery/remote-node-setup) walks through the remote path if you choose it. Mobile wallets use a remote node by default, for the practical reason that a phone can't reasonably store the full chain.

## 5. Fund it, then verify your backup

Before you send anything meaningful into the wallet, do a test restore: install the wallet fresh on a second device (or reinstall it), and restore using only the 25 words you wrote down. If it works, your backup is real. If it doesn't, you've found the problem while the stakes were still zero.

Once you've confirmed the wallet syncs correctly and stays responsive, [How Arqma Wallet syncing actually works](https://arqmawallet.com/how-it-works/syncing) is worth a read if you ever see it stall — and [Arqma Wallet not syncing](https://arqmawallet.com/recovery/wallet-not-syncing) is the fix guide if it does.

## What to read next

- New to the privacy model itself? [Arqma Wallet privacy — the honest version](https://arqmawallet.com/how-it-works/privacy-anonymity)
- Comparing Arqma against wallets you may already know: [Arqma vs Monero](https://arqmawallet.com/how-it-works/arqma-vs-monero), [Arqma vs MetaMask](https://arqmawallet.com/how-it-works/arqma-vs-metamask)
- Questions not covered here: the full [FAQ](https://arqmawallet.com/faq)

---

**Related articles:** [Wallet Types and Platforms](wallet-types-and-platforms.md) · [Seed Phrase and Backups](seed-phrase-and-backups.md) · [Non-Custodial Security Model](non-custodial-and-security-model.md) · [Nodes and Syncing](nodes-and-syncing.md)
