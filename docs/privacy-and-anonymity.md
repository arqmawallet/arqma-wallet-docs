# Privacy and Anonymity: What Arqma Actually Hides

Arqma is a CryptoNote-family privacy coin, which means privacy isn't a feature bolted onto a transparent ledger — it's the default state of every transaction. But "private by default" isn't the same as "invisible in every way," and understanding the difference matters if privacy is the reason you're here.

## What's hidden on-chain

Every Arqma transaction obscures three things simultaneously:

- **The sender**, via ring signatures that blend the real spender in with a group of decoys pulled from the chain, so an outside observer can't isolate which of them actually signed.
- **The receiver**, via one-time stealth addresses generated fresh for each transaction — your public address never appears directly on-chain, so payments to you can't be linked to each other by address alone.
- **The amount**, via RingCT (Ring Confidential Transactions), which hides transaction values while still letting the network validate that no coins were created out of thin air.

The mechanics behind each of these are explained in more depth in [Arqma Wallet architecture, explained](https://arqmawallet.com/how-it-works/architecture), and the honest, no-hype version of what this buys you is in [Arqma Wallet privacy — the honest version](https://arqmawallet.com/how-it-works/privacy-anonymity).

## What's not hidden

This is the part privacy-coin marketing tends to gloss over, so it's worth being direct about it:

- **Your IP address** is visible to whichever node your wallet connects to, unless you route through Tor/i2p or run your own node. A remote node operator can see that *someone* is querying certain addresses, even if they can't see the transaction contents.
- **Timing patterns** — when you check your balance, when you broadcast a transaction — are visible to your connected node regardless of on-chain privacy.
- **Exchange-side KYC** persists on either end of any transaction that touches a regulated exchange. On-chain privacy doesn't retroactively anonymize funds that were tied to your identity before or after they passed through the chain.

None of this is unique to Arqma — it's the general shape of metadata leakage that every privacy-coin wallet has to manage at the network layer rather than the cryptography layer. [What is an Arqma node?](https://arqmawallet.com/how-it-works/nodes) explains why running your own node closes the biggest gap here, and [Set up a remote node in Arqma Wallet](https://arqmawallet.com/recovery/remote-node-setup) covers the setup if you're not ready to run a full node yourself.

## Telemetry and the wallet software itself

Separately from the network layer: official Arqma Wallet builds do not transmit analytics, telemetry, or device fingerprints to any Arqma-operated server. There's no server to send them to in the first place — the project doesn't operate one that collects user data. The project's data-handling stance is laid out plainly in the [privacy notice](https://arqmawallet.com/privacy).

## Putting it together

If your privacy goal is "keep my transaction history from being trivially readable by strangers scanning a public ledger," Arqma's on-chain design handles that by default. If your goal is closer to "leave no trace anywhere in the process," you need to also think about network-layer exposure — which node you trust, whether you're using Tor, and how you acquired the ARQ in the first place. Treating on-chain privacy and operational privacy as the same thing is the most common way people overestimate how anonymous they actually are.

For a broader view of how Arqma's privacy model stacks up against other wallets people commonly compare it to, see [Best non-custodial privacy wallets in 2026](https://arqmawallet.com/how-it-works/best-privacy-wallets) and the head-to-head with the most obvious comparison point, [Arqma vs Monero (XMR)](https://arqmawallet.com/how-it-works/arqma-vs-monero).

---

**Related articles:** [Nodes and Syncing](nodes-and-syncing.md) · [Comparing Arqma to Other Wallets](comparisons.md) · [Non-Custodial Security Model](non-custodial-and-security-model.md) · [Getting Started with Arqma Wallet](getting-started.md)
