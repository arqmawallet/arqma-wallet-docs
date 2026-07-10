# The Non-Custodial Security Model, Explained

"Non-custodial" gets used loosely across crypto marketing, so it's worth being precise about what it actually means for Arqma Wallet, because the term describes a real architectural choice with real consequences — both good and bad.

## What non-custodial actually means

In a custodial setup — an exchange account, for instance — a company holds your private keys on servers it controls, and you access your balance through a login. If the company is compromised, freezes accounts, or shuts down, your access depends on them.

Arqma Wallet works the other way: your spend key and view key are generated on your own device and never leave it. No Arqma contributor, server, or third party ever has access to them. That's the entire definition, and [How non-custodial Arqma Wallet works](https://arqmawallet.com/how-it-works/non-custodial) walks through the technical flow of key generation and storage in more detail. The general concept, independent of any one wallet, is covered in [Non-custodial wallet — explained](https://arqmawallet.com/security/non-custodial).

## The tradeoff nobody should skip past

Self-custody removes a middleman, and it also removes every safety net that middleman would have provided. There's no password-reset email, no support agent who can restore access, no chargeback. If you lose your seed phrase and your wallet file, the funds are gone — not "difficult to recover," gone. [Custodial vs non-custodial wallet — compared](https://arqmawallet.com/security/custodial-vs-non-custodial) lays out this tradeoff without picking a side, because which one is "safer" genuinely depends on your threat model: you're either more worried about a company failing you, or about failing yourself.

## What's actually protecting your funds

A few concrete mechanisms sit underneath the "your keys, your crypto" framing:

- **Local encryption.** Wallet files are encrypted at rest with a password you choose. Even someone with a copy of your `.keys` file can't open it without that password.
- **Signed releases.** Every official release is signed with GPG, with SHA-256 checksums published alongside it, so you can verify that the binary you downloaded matches the public source code rather than trusting the download link blindly.
- **Reproducible builds.** Because the build process is reproducible, independent parties can compile the source themselves and confirm the published binary matches — a stronger guarantee than "trust us."

Whether these mechanisms hold up to outside scrutiny, and what's been reviewed versus what hasn't, is addressed candidly in [Is Arqma Wallet safe? — honest review](https://arqmawallet.com/security/is-arqma-safe) and [Arqma Wallet audits & disclosure](https://arqmawallet.com/security/audits).

## Where the risk actually sits

Because there's no company between you and your funds, the practical risks shift almost entirely onto two things: how you store your seed phrase, and whether you can tell a real Arqma download from a fake one. Neither risk is about the wallet's cryptography — both are about process and vigilance, which is exactly why they're documented separately and in depth: seed handling in [Arqma seed phrase security](https://arqmawallet.com/security/seed-phrase), and fake-download risk in [Phishing protection for Arqma Wallet users](https://arqmawallet.com/security/phishing-protection).

## The short version

Non-custodial means you are the only person who can move your funds — and the only person who can lose access to them. Arqma Wallet's job is to make the cryptography and the storage as sound as possible; the seed phrase discipline is yours to hold up on the other end.

---

**Related articles:** [Seed Phrase and Backups](seed-phrase-and-backups.md) · [Phishing and Staying Safe](phishing-and-safety.md) · [Getting Started with Arqma Wallet](getting-started.md) · [Open Source and the Project](open-source-and-project.md)
