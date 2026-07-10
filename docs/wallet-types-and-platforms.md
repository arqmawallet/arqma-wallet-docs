# Wallet Types and Platforms

Arqma Wallet isn't one piece of software — it's a family of builds that share the same wallet file format and the same 25-word seed, but differ in where they run and how much control they give you. Picking the right one depends on what you're optimizing for: convenience, control, or footprint.

## GUI desktop wallet

The Electron-based GUI wallet is the default recommendation for most people. It bundles both the wallet interface and the option to run a local daemon (`arqmad`), meaning you can go from download to a fully private, self-hosted setup without installing anything separate. The architecture behind this — how the UI, the daemon, and the wallet file relate to each other — is diagrammed in [Arqma Wallet architecture, explained](https://arqmawallet.com/how-it-works/architecture).

It's available for Windows, macOS, and Linux, with platform-specific install steps at [Install on Windows](https://arqmawallet.com/guides/install-windows), [Install on macOS](https://arqmawallet.com/guides/install-macos), and [Install on Linux](https://arqmawallet.com/guides/install-linux).

## CLI wallet

For advanced users, server operators, or anyone integrating Arqma into a script or backend process, the CLI binaries (`arqma-wallet-cli`, `arqma-wallet-rpc`, `arqmad`) offer the lowest footprint and full control over every parameter. There's no UI overhead, and the RPC binary makes it possible to drive the wallet programmatically. This path assumes comfort with a terminal — if that's not you, the GUI wallet does everything the CLI does with a friendlier front end.

## Mobile wallet

The iOS and Android apps are native, lightweight clients that connect to a remote node by default rather than syncing the full chain — a phone doesn't have the storage or bandwidth budget for that. Setup is quick, but the tradeoff is that your chosen remote node can observe some metadata about which addresses you're checking. [Arqma mobile wallet — iPhone & Android setup](https://arqmawallet.com/guides/mobile-setup) covers the install flow, and if you want mobile with desktop-level node privacy, you can point your phone at a node you run yourself — see [Set up a remote node in Arqma Wallet](https://arqmawallet.com/recovery/remote-node-setup).

## Web wallet

A browser-based option exists, but it comes with a different threat model than the native builds: your keys are handled inside a browser tab rather than a dedicated application, which changes what "non-custodial" protects you against. [Is the Arqma web wallet safe?](https://arqmawallet.com/guides/web-wallet) gives an honest answer rather than a marketing one — worth reading before you use it for anything beyond a quick balance check.

## One seed, every platform

Regardless of which build you choose, they all read and write the same 25-word mnemonic format. A wallet created on the GUI can be restored on the CLI, on mobile, or on a fresh install of the GUI on a different computer. This portability is what makes [device switching](https://arqmawallet.com/recovery/device-switching) straightforward and what makes [running multiple wallets](https://arqmawallet.com/recovery/multiple-wallets) on one machine a matter of just using separate wallet files.

Cross-platform support is summarized at [Arqma Wallet runs on every major platform](https://arqmawallet.com/how-it-works/multi-platform), including the specific OS versions tested by contributors.

## How to choose

| If you want... | Use |
|---|---|
| The easiest path, full features, local privacy option | GUI desktop |
| Scripting, automation, minimal resource use | CLI |
| A wallet you carry in your pocket | Mobile |
| A quick browser check, understanding the tradeoffs | Web wallet |

There's no wrong choice here in the sense of losing funds — the wallet file format is universal — but there is a wrong choice in terms of matching the tool to how you actually use crypto day to day. Most people are best served starting with the GUI wallet and layering in CLI or mobile later if a specific need shows up.

---

**Related articles:** [Getting Started with Arqma Wallet](getting-started.md) · [Non-Custodial Security Model](non-custodial-and-security-model.md) · [Nodes and Syncing](nodes-and-syncing.md) · [Wallet Recovery and Troubleshooting](wallet-recovery-and-troubleshooting.md)
