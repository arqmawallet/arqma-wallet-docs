# Seed Phrase and Backups: Doing It Right the First Time

There's exactly one backup that guarantees you can recover an Arqma wallet from nothing: the 25-word seed phrase. Everything else — a password-protected `.keys` file, a cache file, a screenshot you swore you'd delete — is either a convenience or a liability. This article covers what to actually do with the phrase once your wallet shows it to you.

## What the phrase is, technically

The seed phrase is a human-readable encoding of your spend key and view key. Any Arqma Wallet build — GUI, CLI, or mobile — can take those 25 words and rebuild the exact same wallet from them. That portability is the whole point: it's a universal backup format, not a GUI-specific feature. [Arqma seed phrase security](https://arqmawallet.com/security/seed-phrase) covers the generation and display process in detail, including exactly why the wallet only ever shows it to you once.

## Storage, ranked by durability

Not all backup methods survive equally well. In rough order of durability:

1. **Metal stamping or engraving** — survives fire, water, and time in a way paper doesn't.
2. **Pen and paper, stored in two separate physical locations** — the practical minimum, and fine for most people.
3. **A password manager or encrypted file** — better than nothing, but reintroduces a digital attack surface you were trying to avoid.
4. **A cloud note, email draft, or photo** — don't. This is the single most common way seed phrases end up compromised.

The full comparison of storage mediums, with the actual failure modes for each, is in [Where to store your seed phrase safely](https://arqmawallet.com/security/backup-storage). If you want to see how bad backups actually go wrong in practice rather than in theory, [Seven backup mistakes that drain wallets](https://arqmawallet.com/security/backup-mistakes) catalogues real failure patterns — most of them boring, none of them exotic.

## Backing up more than just the seed

Beyond the seed phrase, your `.keys` file and cache file are also backup-relevant:

- The **`.keys` file** is encrypted with your wallet password and can restore the wallet without the seed phrase — provided you also still have that password. It's a useful secondary backup, not a replacement for the seed.
- The **cache file** is purely a performance optimization for resync speed. It's not required for recovery and isn't worth stressing over.

[How to back up your Arqma Wallet](https://arqmawallet.com/security/backup-wallet) walks through backing up both files alongside the seed phrase, and [Securing your Arqma Wallet .keys file](https://arqmawallet.com/security/wallet-file-security) goes deeper on protecting that file specifically if you choose to rely on it.

## Verify before you trust it

A backup you haven't tested is a guess. Before moving meaningful funds into a wallet, do a real restore: install fresh on a second device, or wipe and reinstall on the same one, and rebuild the wallet using only your written-down seed phrase. If the addresses and balance match, your backup works. This single habit prevents the single most common cause of permanent fund loss — discovering a backup mistake only after it's too late to fix.

## If it's already too late

If you've lost the seed phrase and don't have the `.keys` file and password either, there's no way around it: the funds are permanently inaccessible. No exchange, no Arqma contributor, and no third-party "recovery service" can restore them — and anyone claiming otherwise is running a scam targeting people in exactly this situation. If you're in this position, [Lost your Arqma backup — what now?](https://arqmawallet.com/recovery/lost-backup) is worth reading in full before you interact with anyone offering to "help."

---

**Related articles:** [Non-Custodial Security Model](non-custodial-and-security-model.md) · [Wallet Recovery and Troubleshooting](wallet-recovery-and-troubleshooting.md) · [Phishing and Staying Safe](phishing-and-safety.md) · [Getting Started with Arqma Wallet](getting-started.md)
