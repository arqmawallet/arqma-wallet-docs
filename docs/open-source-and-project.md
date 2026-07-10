# Open Source and the Arqma Project

Understanding who actually builds and maintains Arqma Wallet changes how you should think about trust, support expectations, and what "official" even means for a project like this.

## There's no company

Arqma has no foundation, no venture capital investment, and no public token sale behind it. Development happens in the open on GitHub, with code review carried out by volunteer contributors rather than salaried employees. That's not a minor detail — it shapes everything downstream: why there's no customer support line, why marketing claims should be read skeptically (there's no PR department polishing them), and why verifying things yourself (checksums, source code, release signatures) matters more than it would with a venture-backed competitor. [About the Arqma project (ARQ)](https://arqmawallet.com/about) covers the project's history and structure in full.

## The coin and the wallet are two different things

A common point of confusion: "Arqma" refers to both the ARQ blockchain network itself and the wallet software used to interact with it. They're related but distinct — the network is the protocol and the ledger; the wallet is client software that lets you hold and transact ARQ, and it's not the only such client that could theoretically exist. [Arqma coin vs Arqma Wallet — explained](https://arqmawallet.com/about/coin-vs-wallet) untangles this distinction clearly if you've seen the two terms used interchangeably and weren't sure whether that was accurate.

## What "open source" buys you

Every meaningful part of Arqma Wallet — the GUI, the CLI tools, the daemon — has its source published on GitHub, under the `arqma` organization. This matters in a very concrete way: it means the reproducible build process mentioned throughout the security documentation isn't a marketing claim you have to take on faith. Anyone with the technical background can clone the repository, compile it themselves, and compare the result against the officially published binary. [Open-source Arqma Wallet — the code](https://arqmawallet.com/how-it-works/open-source) walks through what's public, where, and how to go about that verification if you want to do it yourself.

## Community over corporate support

Because there's no company, there's also no traditional customer support in the sense of a ticketing system with SLAs. Instead, help flows through the same open channels the code does — GitHub issues and discussion for anything technical, and the project's X account for announcements and community discussion. [Arqma community & support](https://arqmawallet.com/community) is the map of where those channels actually live, and [How to get Arqma Wallet help safely](https://arqmawallet.com/getting-help) covers how to ask for help there without exposing anything you shouldn't.

## Why this structure matters for trust

A community-run, open-source project without a company behind it cuts both ways. There's no single point of corporate failure that could shut the project down or compromise it from the inside — but there's also no company whose reputation is on the line to reassure you, which is exactly why the project leans so heavily on things that can be independently verified: signed releases, published checksums, reproducible builds, and open code. If you're the kind of user who wants to verify rather than trust, this structure gives you the tools to actually do that. If you'd rather have a company standing behind the product, that's a legitimate preference too — and it's worth being honest with yourself about which one you are, since it should inform whether Arqma is the right wallet for you at all.

---

**Related articles:** [Non-Custodial Security Model](non-custodial-and-security-model.md) · [Phishing and Staying Safe](phishing-and-safety.md) · [Comparing Arqma to Other Wallets](comparisons.md) · [Getting Started with Arqma Wallet](getting-started.md)
