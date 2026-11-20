---
title: "Pear and the Holepunch stack"
description: "Peer-distributed applications, code, and data using Hypercore."
---

# Pear and the Holepunch stack

**Assessment:** Conditional ecosystem / application development platform.  
**Maturity:** Active platform; individual applications vary. **Reviewed:** 2026-11-19.

[Pear documentation](https://docs.pears.com/) · [Storage and distribution](https://docs.pears.com/pear/explanation/storage-and-distribution/) · [Peer-to-peer modules](https://docs.pears.com/p2p/)

Pear is more than a browser for distributed pages. It is a runtime for packaged applications that can be installed from `pear://` identifiers and served from peers. Software releases can be seeded by developers and replicated by other devices, rather than requiring a central download website.

## What can be built or used?

- Desktop and CLI applications shipped over peer distribution.
- Applications using [Hypercore](https://docs.pears.com/p2p/) replicated append-only records, Hyperdrive file trees, or Hyperbee indexed data.
- Messaging and collaboration, such as the existing [Keet](https://keet.io/) entry, which should have its own architectural assessment.

## How does state persist?

Application bytes and updates live in Hyperdrive/Hypercore feeds. Peers can seed them; ordinary devices can replicate both application code and user-generated data when the application implements that behaviour. This is stateful replication rather than a transient point-to-point file exchange.

## Unresolved two-device dependencies

Establish whether independent peer discovery and application installation require default public DHT bootstrap nodes, an external signalling/relay provider, or a permanent seeder. Test two existing installations exchanging an application and replicated data when the original publisher is offline, with no dedicated third machine. **No actual two-device test has been performed for this catalog entry.**

Do not promote every application built using Pear automatically. Supporting libraries and accessory tools should remain on this page.
