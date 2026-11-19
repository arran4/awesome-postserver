---
title: "How entries are assessed"
description: "Record what was verified, in which mode, and when."
---

# Assessment method

**Assessment date: 2026-11-19.** Each entry is evaluated for a *specific working mode*, not for all capabilities a project advertises. Historic and existing entries may predate this policy.

## Architecture: a two-device test

Start with one desktop and one phone (or two ordinary user devices), both able to run the client. Remove dedicated servers, fixed home servers, special network appliances, always-on mailboxes and compulsory third-party relays. Does the useful core mode still work, and where is meaningful persistent state stored? A local bundled daemon on a participating device is permitted. Peer presence and connectivity still matter; failure without a network path is not automatically disqualifying.

## Distinct fields

| Field | Values | Meaning |
| --- | --- | --- |
| Assessment | Qualifies / Conditional / Supporting / Excluded | Depends on the particular tested mode |
| Maturity | Alpha / Beta / Stable / Legacy / Unverified | Project readiness, independent of architecture |
| Reviewed | YYYY-MM-DD | When claims and official sources were checked |
| Peer discovery | LAN, direct address, DHT, invitations, manual, other | How devices locate each other |
| Persistent state | Local records, replicated records, bundles, none | Whether this is more than transient transport |
| Mandatory dependencies | Explicit named services or none established | Include bootstrap, relay, naming and account services |

A durable one-off file handoff is presently **unresolved** as an eligibility boundary. Do not silently treat it as either a qualifying stateful application or an automatic exclusion.

## Evidence in pull requests

Document the core task a user performs, who owns records, what happens when peers disconnect, whether ordinary peers can relay, whether a dedicated service is required, and which claims were actually tested. Cite official documentation and implementations. Disclose limitations and unresolved architecture questions rather than translating product claims like “decentralized” into guarantees.

## Ecosystem pages

A platform page can describe a protocol, running node, applications, libraries and accessory tools together. Distinguish truly qualifying programs from programs that merely consume the network or require additional infrastructure. Supporting technologies need not themselves be recommended as standalone Post-Server applications.
