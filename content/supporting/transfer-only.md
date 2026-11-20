---
title: "Transfer-only tools: inclusion boundary"
description: "How to assess one-off file handoff versus durable peer-owned state."
---

# Transfer-only tools — unresolved inclusion boundary

**Assessment:** Provisional supporting tools; policy decision pending. **Reviewed:** 2026-11-19.

Ordinary LAN transfer utilities are server-optional, but they may do nothing more than hand bytes from one device to another. They generally do not maintain a persistent shared dataset, reconcile revisions or carry messages over multiple disconnections. Including every such tool would risk turning the main catalog into an unlimited list of point-to-point sockets.

## Two defensible rules

- **Rule A — replicated or persistent shared application state:** list transfer-only utilities on this supporting page, not the main application catalog.
- **Rule B — durable payload handoff counts:** a tool that permanently transfers files between user devices may qualify, even without repeated synchronization. This would admit many more utilities.

**Neither is settled.** The main list should not quietly adopt one interpretation through individual PRs.

## Candidate utilities

- [LocalSend](https://localsend.org/) — local cross-platform file transfer; proposed separately in existing [PR #11](https://github.com/arran4/awesome-postserver/pull/11).
- [NearDrop](https://github.com/grishka/NearDrop) — receives Android Quick Share transfers on macOS.
- [Sharik](https://github.com/marchellodev/sharik) — cross-platform LAN file sharing, with current maintenance to verify.
- [Warpinator](https://github.com/linuxmint/warpinator) — local peer discovery and transfers; already tracked in [candidate issue #19](https://github.com/arran4/awesome-postserver/issues/19).

## Before classifying

Choose the rule; then describe each application's ordinary mode, stored artifacts, whether it serves content over time, and whether a third service is required. Keep useful accessories discoverable even when they are excluded from the primary catalog.
