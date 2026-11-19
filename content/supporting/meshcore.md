---
title: "MeshCore and MeshOS"
description: "Companion radios, repeaters, room servers and AirLink peer messaging."
---

# MeshCore and MeshOS

**Assessment:** Conditional / supporting until the specific mode meets the two-device test.  
**Maturity:** Active ecosystem; device/firmware-specific. **Reviewed:** 2026-11-19.

[MeshCore project](https://meshcore.co.uk/) · [Device roles](https://www.meshcore.cz/en:zacinam:role) · [MeshOS AirLink announcement](https://meshcore.co.uk/blog/introducing-meshos-airlink.html)

MeshCore is a LoRa packet-messaging ecosystem with different radio roles. A **companion** participates in messages; ordinary companion radios can communicate directly while in range. **Repeaters** forward packets across additional hops, while **room servers** store and return room message history. A repeater or room server generally has a specialized role instead of being just another ordinary companion.

## Two separate behaviours

1. **Direct companion chat:** No separate repeater is required when the companion radios can reach each other. Locally retained history may be useful, but ordinary local chat alone is not enough to assume shared peer state.
2. **Shared offline room history:** Dedicated room servers store posts for later retrieval. If a third server device is mandatory for the claimed feature, it does **not** satisfy server-optional requirements.

## MeshOS AirLink merits a new test

MeshOS advertises Bluetooth mesh communication with **store-and-forward** and bridging to MeshCore. This may allow useful stateful, intermittent phone-to-phone messaging without a LoRa repeater or separate always-on room server. The specific implementation, supported client devices, durability, and relay behaviour need to be verified; do not dismiss the whole ecosystem based only on the older LoRa roles.

## Proposed acceptance test

Use two ordinary supported companion devices with no repeater and no room server. Exchange messages, disconnect, restart if appropriate, reconnect and verify stored delivery. Determine whether a third dedicated AirLink gateway is required for any advertised multi-hop functionality. Record the firmware/app version tested.

**Not yet a main catalog entry.**
