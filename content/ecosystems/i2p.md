---
title: "I2P"
description: "An anonymous peer-operated overlay, with special bootstrap and network-database roles."
---

# I2P

**Assessment:** Conditional ecosystem, not yet verified as a strict two-device deployment.  
**Maturity:** Established network; individual apps vary. **Reviewed:** 2026-11-19.

[Project](https://geti2p.net/) · [Network database and reseeding](https://geti2p.net/en/docs/how/network-database) · [FAQ](https://geti2p.net/en/faq)

I2P (*Invisible Internet Project*) is an encrypted overlay of locally run routers. Each user can run a router as a participant, and other participating routers may forward encrypted traffic. Applications can offer websites, messaging and storage over destinations within this overlay. I2P is not itself a conventional mail or file synchronization application.

## What is stored?

A router maintains a local network database of peer routing records and destination leases. A changing subset of higher-capacity routers acts as **floodfill** nodes that replicate routing records. This is distributed discovery state; actual content persistence depends on the application. In particular, the existing [I2P-Bote](https://github.com/i2p/i2p.i2p-bote) entry needs its own lifecycle and two-device check.

## Which infrastructure is required?

A new router normally fetches initial router records from volunteer **reseed servers** on the normal internet. This is not the only way to supply records: a participating router can export them for another user. Floodfill participants may come and go, but routers generally rely on the wider I2P network for tunnel diversity. Neither fact is proof that ordinary two-device use works in isolation.

## Decision before main-list inclusion

Show two ordinary routers obtaining peers manually or without a mandatory third service, and demonstrate a real persistent I2P application. Confirm whether two devices can operate the required tunnel and network-database roles at usable reliability; document any loss of anonymity when the network is small.

Multilingual implementations may be useful evidence of protocol interoperability, but **language count is not the inclusion rule**.
