# Frequently Asked Questions, Digested

The full [FAQ](https://arqmawallet.com/faq) on the site covers the questions people ask most. This is a shorter digest of the ones worth knowing before you install anything, with links to the deeper guide behind each answer.

## Is Arqma Wallet free?

Yes — it's open-source software with no purchase price, subscription, or hidden fee. The only cost involved is the standard network transaction fee any blockchain wallet pays to send funds.

## Is it custodial?

No. Keys are generated and stored entirely on your device; nobody else — not the project, not a server — ever has access to them. See [How non-custodial Arqma Wallet works](https://arqmawallet.com/how-it-works/non-custodial) for the full mechanics.

## What does it support besides ARQ?

Nothing — it's a single-chain wallet for the Arqma network only, with no multi-chain support and no smart-contract layer. If you need a multi-asset wallet, see the [comparison with Trust Wallet](https://arqmawallet.com/how-it-works/arqma-vs-trust-wallet) and [MetaMask](https://arqmawallet.com/how-it-works/arqma-vs-metamask) for how those differ in scope.

## Can a lost seed phrase be recovered?

No. The 25-word mnemonic is the sole master backup, with no reset mechanism. Anyone offering paid "crypto recovery services" for a lost seed is running a scam. [Lost your Arqma backup — what now?](https://arqmawallet.com/recovery/lost-backup) covers this scenario directly.

## Does it require KYC?

No — there's no account, no email signup, and no identity verification anywhere in the wallet software itself. (Note that exchanges you use to acquire ARQ may have their own KYC requirements — that's outside the wallet's scope.)

## Which platforms are supported?

Windows 10/11, macOS (Intel and Apple Silicon), Linux (x86_64), Android 8+, and iOS 14+. Install steps per platform: [Windows](https://arqmawallet.com/guides/install-windows), [macOS](https://arqmawallet.com/guides/install-macos), [Linux](https://arqmawallet.com/guides/install-linux), [mobile](https://arqmawallet.com/guides/mobile-setup).

## How is Arqma different from Monero?

Both are CryptoNote privacy coins with the same core privacy primitives. Arqma is a smaller 2018 fork with a CPU-friendly mining algorithm and a hybrid PoW+PoS consensus model; Monero has a much larger network and anonymity set. Full comparison: [Arqma vs Monero (XMR)](https://arqmawallet.com/how-it-works/arqma-vs-monero).

## Does the wallet collect telemetry?

No. Official builds don't transmit analytics or device data to any Arqma-operated server — see the [privacy notice](https://arqmawallet.com/privacy) for the project's data-handling stance in full.

## How is a release verified?

Every release publishes a SHA-256 checksum and a GPG signature on the GitHub release page. Verifying both before installing is the main defense against fake or tampered downloads — see [Phishing protection for Arqma Wallet users](https://arqmawallet.com/security/phishing-protection).

## Where can I get help?

The project's GitHub and X account (@ArqmaNetwork) are the legitimate channels — see [Arqma community & support](https://arqmawallet.com/community) and [How to get Arqma Wallet help safely](https://arqmawallet.com/getting-help). No legitimate helper will ever ask for your seed phrase.

---

**Related articles:** [Getting Started with Arqma Wallet](getting-started.md) · [Non-Custodial Security Model](non-custodial-and-security-model.md) · [Seed Phrase and Backups](seed-phrase-and-backups.md) · [Phishing and Staying Safe](phishing-and-safety.md)
