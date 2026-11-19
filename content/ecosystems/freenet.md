---
title: "Freenet (new)"
description: "A local peer-run platform for distributed applications."
---

# Freenet (new)

**Assessment:** Conditional — architecture matches the Post-Server goal; the strict two-device demonstration and bootstrap dependencies still require verification.  
**Maturity:** Alpha. **Reviewed:** 2026-11-19.

[Official site](https://freenet.org/) · [Getting started](https://freenet.org/quickstart/) · [Platform architecture](https://freenet.org/build/manual/introduction/)

The current Freenet project is a platform for applications whose code and shared state propagate through participating peers. A local background peer runs on the user's computer; a browser talks to that *local participant*, rather than a fixed central application website. Running a local service as part of the participant is acceptable under the catalog policy.

## What can you do?

- [River](https://freenet.org/river/) — group chat. See the [River catalog page]({{< relref "/applications/river.md" >}}).
- [Delta](https://freenet.org/apps/) — distributed publishing.
- [Atlas](https://freenet.org/apps/) — discovery and search.
- [freenet-git](https://freenet.org/apps/) — Git operations over Freenet.

These are distinct applications on one platform; their stability and mandatory dependencies should be assessed independently.

## Two-device and persistence check

The local peer stores and exchanges application information as part of a peer-run network. A planned acceptance test is two independently installed ordinary peers exchanging a River room and its history after restart or temporary disconnection, with no third permanently available service. **This test has not yet been executed for this entry.** Determine whether join/bootstrap requires a third-party service and whether it is genuinely optional.

## Avoid name confusion

The *original* Freenet project is now known as [Hyphanet](https://www.hyphanet.org/). It is a distinct system with its own distributed content network, and should not be conflated with new Freenet.
