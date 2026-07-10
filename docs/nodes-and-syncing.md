# Nodes and Syncing

Every crypto wallet needs some way to see the current state of the blockchain, and how it gets that view — local or remote — is one of the more consequential setup decisions in Arqma Wallet, both for privacy and for day-to-day usability.

## Local node vs. remote node

A **local node** means your desktop wallet downloads and independently verifies the entire Arqma blockchain itself, running the `arqmad` daemon that ships bundled with the GUI wallet. Nothing about your wallet activity is visible to anyone else, because there's no "anyone else" in the loop — you're your own source of truth.

A **remote node** means your wallet connects to someone else's already-synced node over the network and asks it for blockchain data. This is much faster to set up (no initial multi-gigabyte sync) and lighter on your disk, but it means that node operator can see connection metadata about your wallet's queries, even though they can't see your private keys or decrypt your transactions.

[What is an Arqma node?](https://arqmawallet.com/how-it-works/nodes) breaks this tradeoff down in full, and it's the right first read if you're deciding which path to take. Mobile wallets use a remote node by default, simply because a phone isn't a practical place to store the full chain.

## Setting up a remote node

If you've chosen the remote path — or you're on mobile, where it's the only path — [Set up a remote node in Arqma Wallet](https://arqmawallet.com/recovery/remote-node-setup) covers entering a node address in the wallet settings, what to look for in a trustworthy public node, and how to point your wallet at a node you run yourself if you want mobile convenience with desktop-level trust.

## How syncing actually works

Once connected — local or remote — your wallet needs to scan the blockchain for transactions belonging to your addresses. This is where most "the wallet feels broken" reports actually come from: syncing is working, just slowly, and it looks identical to being stuck. [How Arqma Wallet syncing actually works](https://arqmawallet.com/how-it-works/syncing) explains what the wallet is doing block by block and roughly how long each stage should take on typical hardware.

## When it doesn't sync

If your wallet has been sitting at the same block height for an unreasonable amount of time, two guides cover the practical troubleshooting:

- [Arqma Wallet not syncing](https://arqmawallet.com/recovery/wallet-not-syncing) — a five-step diagnostic for wallets that appear stuck outright, covering the common causes: a dead remote node, a firewall blocking the daemon's ports, or a corrupted local chain that needs a resync.
- [Why Arqma Wallet feels slow — and how to fix it](https://arqmawallet.com/recovery/fix-slow-wallet) — for wallets that are syncing but painfully slowly, which is usually a disk I/O or node-choice problem rather than anything wrong with the wallet itself.

## A practical rule of thumb

If you're running the desktop GUI wallet and privacy is your priority, run a local node once and let it fully sync — it's a one-time cost. If you're mostly checking balances and sending occasional payments and don't want to manage node infrastructure, a well-chosen remote node is a reasonable and common tradeoff, especially if you pair it with Tor for the connection itself. Mobile users are on remote nodes by default and can upgrade to pointing at a self-hosted node later without losing anything, since the wallet file itself doesn't change.

---

**Related articles:** [Privacy and Anonymity](privacy-and-anonymity.md) · [Getting Started with Arqma Wallet](getting-started.md) · [Wallet Recovery and Troubleshooting](wallet-recovery-and-troubleshooting.md) · [Wallet Types and Platforms](wallet-types-and-platforms.md)
