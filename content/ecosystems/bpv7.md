---
title: "Bundle Protocol Version 7"
description: "Delay-tolerant storage and forwarding across intermittently connected nodes."
---

# Bundle Protocol Version 7 (BPv7)

**Assessment:** Supporting protocol ecosystem; implementations can build qualifying applications.  
**Maturity:** Standardized protocol; implementation maturity varies. **Reviewed:** 2026-11-19.

[Published standard — RFC 9171](https://www.rfc-editor.org/rfc/rfc9171) · [dtn7-go](https://github.com/dtn7/dtn7-go) · [dtn7-rs](https://github.com/dtn7/dtn7-rs)

BPv7 defines discrete *bundles* that nodes can retain, carry and forward across connectivity gaps. Unlike a live socket or video stream, a bundle represents persistent transferable content with routing and lifetime metadata. End-to-end connectivity need not exist at the moment a sender hands a bundle to its next hop.

## Applications and implementations

- **dtn7-go:** Go implementation and daemon components for forwarding and application integration.
- **dtn7-rs:** independent Rust implementation of BPv7.
- More end-user software should be listed here **only when actual runnable applications are identified**, not inferred from protocol capabilities.

## Why this differs from WebRTC

WebRTC establishes transport sessions. BPv7 explicitly models durable messages and asynchronous forwarding; its node implementation owns queued state. BPv7 still does **not** by itself provide an end-user conversation or collaborative application.

## Two-device demonstration to verify

Run ordinary BPv7 nodes on two devices; create a bundle when only the sender is present; bring peers into contact and deliver it without an independently managed central router or relay. Verify local persistent storage, contact configuration and any hard-coded discovery/service dependencies. No test is claimed to have been executed for this assessment.

**Catalog placement:** ecosystem/developer foundation, not a primary end-user application.
