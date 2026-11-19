---
title: "OpenBazaar"
description: "Peer-operated marketplace storefronts, old and new designs."
---

# OpenBazaar — local-node marketplace

**Assessment:** Conditional application family; two-device mode and service dependencies not tested.  
**Maturity:** Original 2.0 implementation historical; newer work separately experimental. **Reviewed:** 2026-11-19.

[Original OpenBazaar Go daemon](https://github.com/OpenBazaar/openbazaar-go) · [Original desktop client](https://github.com/OpenBazaar/openbazaar-desktop) · [Current project and research](https://www.openbazaar.org/)

The historic OpenBazaar desktop application could run a **local OpenBazaar daemon**, rather than depending on a remote server hosting every user's store. Its daemon embedded a modified IPFS node to distribute signed listings and other marketplace data. The word “server” in the daemon's name does not make it an independently required server, because it could run on an ordinary participant's device.

## The distinction that matters

- **Potentially qualifying:** a buyer and seller each run the ordinary app and their local node; the seller creates a persisted catalog and the buyer retrieves it from peers without a permanent special store host.
- **Disqualifying mode:** a mobile client that works only by accessing a separately provisioned, always-on shop server; or a marketplace whose mandatory directory, storage or relay is not provided by ordinary participants.

Financial transactions, escrow/moderation and any required external blockchain services deserve **separate** discussion; successful browsing does not prove a complete independent trade.

## Versions and next tests

The original 2.0 stack and its more recent successor work must not be represented as one maintained product. Verify which installation and network are actually runnable in 2026, which side holds durable listings, what bootstraps peer discovery, and whether a third server must remain online.

Do not promote the current project to the main list or label it Stable until the specific app version and two-device flow have been demonstrated.
