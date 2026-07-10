# Wallet Recovery and Troubleshooting

Most Arqma Wallet issues fall into a small number of predictable categories: restoring on a new device, a transaction that seems stuck, a wallet that won't sync, or trying to figure out whether something is broken versus just working normally but slowly. This article is a map to the right guide for each.

## Restoring from your seed phrase

If you're setting up on a new device, reinstalling after a wipe, or deliberately testing a backup, [Arqma Wallet recovery — step by step](https://arqmawallet.com/recovery/wallet-recovery) is the full walkthrough: install the wallet, choose "restore from seed" instead of "create new," and enter your 25 words in order. The wallet then rebuilds your keys and begins rescanning the chain to rebuild your transaction history — this rescan is normal and can take a while depending on how far back your wallet's history goes.

If you have the seed phrase but something about the restore isn't behaving as expected, cross-check against [Restoring Arqma Wallet from the .keys file](https://arqmawallet.com/recovery/wallet-file-recovery), which covers the alternate restore path using your encrypted wallet file and password instead of the seed — useful if you have both and want to compare results, or if the `.keys` file is actually what you're trying to recover from.

## Moving to a new device

Switching phones or computers doesn't require anything exotic — the seed phrase (or the `.keys` file plus password) is portable by design. [Move Arqma Wallet to a new device](https://arqmawallet.com/recovery/device-switching) covers the safe order of operations: verify the new install works with your restored seed before wiping or discarding the old device, so you're never in a position where neither device has a working wallet.

## Running more than one wallet

Some users legitimately want separate wallets on one machine — for example, separating funds by purpose. This is straightforward since each wallet is just its own file pair, and [Running multiple Arqma Wallets on one device](https://arqmawallet.com/recovery/multiple-wallets) covers naming conventions and avoiding the most common mistake, which is accidentally overwriting one wallet file with another during setup.

## Stuck or pending transactions

A transaction that's been "pending" longer than expected is unsettling but usually explainable — typically a fee/priority mismatch or a temporarily congested network rather than a lost transaction. [Arqma transaction stuck — what to do](https://arqmawallet.com/recovery/transaction-troubleshooting) covers how to check a transaction's actual status versus what your wallet UI is showing, and when (if ever) it's appropriate to resend.

## Sync problems

If the wallet isn't the problem but its connection to the network is, that's a separate troubleshooting path covered in [Arqma Wallet not syncing](https://arqmawallet.com/recovery/wallet-not-syncing) and, for a wallet that syncs but crawls, [Why Arqma Wallet feels slow — and how to fix it](https://arqmawallet.com/recovery/fix-slow-wallet). Both are downstream of the node concepts in [What is an Arqma node?](https://arqmawallet.com/how-it-works/nodes).

## If the seed phrase itself is gone

Every path above assumes you still have your seed phrase or your `.keys` file and password. If neither survived, the situation is categorically different — there is no technical recovery path, full stop. [Lost your Arqma backup — what now?](https://arqmawallet.com/recovery/lost-backup) explains why, and warns specifically about the scam ecosystem that targets people searching for a way around this.

## Quick reference

| Problem | Guide |
|---|---|
| Setting up on a new device | [Device switching](https://arqmawallet.com/recovery/device-switching) |
| Restoring from your 25 words | [Wallet recovery](https://arqmawallet.com/recovery/wallet-recovery) |
| Restoring from the .keys file | [Wallet file recovery](https://arqmawallet.com/recovery/wallet-file-recovery) |
| Wallet won't sync at all | [Wallet not syncing](https://arqmawallet.com/recovery/wallet-not-syncing) |
| Wallet syncs but is slow | [Fix a slow wallet](https://arqmawallet.com/recovery/fix-slow-wallet) |
| Transaction stuck pending | [Transaction troubleshooting](https://arqmawallet.com/recovery/transaction-troubleshooting) |
| Seed phrase lost entirely | [Lost your backup](https://arqmawallet.com/recovery/lost-backup) |

---

**Related articles:** [Seed Phrase and Backups](seed-phrase-and-backups.md) · [Nodes and Syncing](nodes-and-syncing.md) · [Wallet Types and Platforms](wallet-types-and-platforms.md) · [Phishing and Staying Safe](phishing-and-safety.md)
