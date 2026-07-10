# Phishing Protection and Staying Safe

In a non-custodial wallet, the cryptography isn't usually where people get hurt — the social engineering is. Fake download pages, lookalike domains, and impersonated "support" are the actual attack surface for most Arqma Wallet users, and they're entirely avoidable once you know the pattern.

## Fake downloads and lookalike domains

Because Arqma Wallet is open source and unaffiliated with any company, there's no single centralized authority actively hunting down copycat download sites the way a large corporation's legal team might. That makes verifying your download source your responsibility, not a background guarantee.

The two sources worth trusting are the official website's download page and the project's GitHub release page — nowhere else. Every legitimate release ships with a SHA-256 checksum and a GPG signature; if a download page doesn't offer either, that's already a red flag. [Phishing protection for Arqma Wallet users](https://arqmawallet.com/security/phishing-protection) covers the specific patterns fake sites tend to use — urgency, close-but-not-quite domain names, "download accelerator" wrappers — and how to check a checksum yourself before running an installer.

## No one from Arqma will ever ask for your seed phrase

This is worth stating plainly because it's the single most effective phishing angle across all of crypto, not just Arqma: **no legitimate support channel, contributor, or "recovery service" will ever ask you for your 25-word seed phrase.** Anyone who does — over X/Twitter DM, email, a Discord ticket, a phone call — is attempting to steal your funds, regardless of how official they sound or how urgent they make it seem. If someone asks, the conversation is over; don't explain, don't negotiate, just stop responding.

## Getting real help without exposing yourself

If you actually need support, [How to get Arqma Wallet help safely](https://arqmawallet.com/getting-help) covers where legitimate help exists — the project's GitHub and its official X account — and what information is safe to share with a helper (transaction IDs, error messages, wallet version) versus what never is (seed phrase, private keys, wallet password).

The broader community and support channels are listed at [Arqma community & support](https://arqmawallet.com/community), which is also the right place to verify that a channel claiming to be "official" actually is.

## "Recovery service" scams specifically

A particular scam pattern worth calling out on its own: services that advertise the ability to recover a lost seed phrase or hacked wallet for a fee. Because of how the seed phrase system works, this is not a real capability — no service, however credible-looking, can reconstruct keys that were never generated with their involvement. Anyone advertising this is either running an outright scam or, at best, attempting to get you to hand over information (like a partial seed or wallet file) that lets them steal what's left. If you're in a position where you've lost access and are searching for a way back in, read [Lost your Arqma backup — what now?](https://arqmawallet.com/recovery/lost-backup) before engaging with anyone offering to help for payment.

## A short checklist

- Only download from [arqmawallet.com/download](https://arqmawallet.com/download) or the official GitHub release page.
- Verify the SHA-256 checksum and GPG signature before running an installer.
- Never type your seed phrase into a website, chat, or any app other than a wallet you launched yourself.
- Treat any unsolicited "support" contact as hostile until proven otherwise.
- If something feels engineered to rush you, that's the tell — slow down.

For the bigger picture of how these individual risks fit into the wallet's overall security posture, see [Is Arqma Wallet safe? — honest review](https://arqmawallet.com/security/is-arqma-safe).

---

**Related articles:** [Non-Custodial Security Model](non-custodial-and-security-model.md) · [Seed Phrase and Backups](seed-phrase-and-backups.md) · [Wallet Recovery and Troubleshooting](wallet-recovery-and-troubleshooting.md) · [Open Source and the Project](open-source-and-project.md)
