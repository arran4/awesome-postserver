---
title: "Nostr (relay-dependent by design)"
description: "Signed social events published via relays, with possible future peer-hosted variants."
---

# Nostr and relay-dependent clients

**Assessment:** Supporting / excluded from the core application list in its ordinary operating mode.  
**Maturity:** Established protocol with varied clients. **Reviewed:** 2026-11-19.

[Nostr protocol repository](https://github.com/nostr-protocol/nips) · [NIP-01](https://github.com/nostr-protocol/nips/blob/master/01.md)

Nostr clients typically publish signed events to and retrieve them from WebSocket relays. Relays are replaceable and decentralized, but normal client software still **requires at least one separately operating relay** to share messages. Replaceable is not the same as optional.

## What would qualify?

A specific client could qualify if ordinary participating devices also operate relays or exchange their retained event state **directly**, without mandatory independent infrastructure. Such a mode needs direct evidence, not merely a self-hostable Nostr relay or a public relay list.

This is a protocol and accessory reference, **not a claim that all possible Nostr implementations are impossible to run without external servers**. New clients with integrated peer-owned relay and persistence may warrant a separate application entry.

See [Contributing](https://github.com/arran4/awesome-postserver/blob/main/CONTRIBUTING.md) for the two-device criterion.
