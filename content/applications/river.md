---
title: "River"
description: "Group chat operating on locally run Freenet peers."
---

# River

**Assessment:** Conditional — promising stateful Post-Server chat; no independent strict two-device test recorded here.  
**Maturity:** Alpha. **Reviewed:** 2026-11-19.

[Official River page](https://freenet.org/river/) · [Install Freenet and run River](https://freenet.org/quickstart/) · [Freenet applications](https://freenet.org/apps/)

River provides group chat on the **new Freenet** platform. Each participant installs a Freenet peer locally; the River interface uses that peer. Rather than connecting to a separately hosted chat server, rooms and messages propagate through the participating network. Room state can persist beyond the original creator's online session.

## Why it is interesting

- **Useful persistent state:** chat rooms and their message history, not just a transient connection.
- **Participant-operated:** a Freenet peer runs as part of each ordinary installation.
- **No dedicated application server asserted:** a separate always-on room service is not part of the advertised architecture.

## Verification before listing as qualified

Install two ordinary peers, exchange messages in a room, restart the local applications, and verify room persistence and reconnect behaviour. Identify any mandatory discovery/bootstrap dependencies, and distinguish peer replicas from optional wider-network availability. Until those questions are answered, do not present guaranteed operation with only two isolated peers.

See also [Freenet's ecosystem](https://freenet.org/apps/). River's alpha status should remain visible regardless of architectural suitability.
