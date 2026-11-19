---
title: "Holochain"
description: "Participant-operated application conductors with current bootstrap infrastructure needs."
---

# Holochain

**Assessment:** Supporting / conditional application platform; do not assert strict server-optional use by default.  
**Maturity:** Active development. **Reviewed:** 2026-11-19.

[Build guide](https://developer.holochain.org/build/) · [Application architecture](https://developer.holochain.org/concepts/2_application_architecture/) · [Operating an hApp](https://developer.holochain.org/build/operating-a-happ/) · [Network infrastructure](https://developer.holochain.org/resources/howtos/running-network-infrastructure/)

Holochain applications (*hApps*) execute on a local **conductor** process and maintain participant-owned source chains, with data exchanged through peers. The conductor is an application-local service on the participant's own device, not inherently a disqualifying dedicated server.

## The unresolved infrastructure problem

Current deployment documentation covers explicitly provisioned bootstrap and relay infrastructure; the 0.7 architecture has changed in relation to earlier signal/ICE terminology. A design that distributes data among users can still rely on a mandatory **separate rendezvous/relay service**. That is not compliant with the catalog's strict two-device rule.

## Research needed

Test whether two ordinary conductors on a LAN can find each other, exchange and retain hApp state, restart, and reconnect without a third-party bootstrap service. If the answer is yes only in a custom test harness or special configuration, describe the precise mode instead of listing ordinary Holochain apps as universally qualifying.

Individual hApps should be assessed separately. Do not confuse the platform's local persistence with proof that required discovery is server-optional.
