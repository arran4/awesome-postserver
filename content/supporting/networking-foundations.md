---
title: "Networking foundations"
description: "Enabling transports, discovery and infrastructure—not automatically qualifying applications."
---

# Networking foundations

**Assessment:** Supporting technologies. **Reviewed:** 2026-11-19.

These tools can help build server-optional software, but networking a pair of machines is not equivalent to persisting or replicating meaningful application state.

| Technology | Contribution | Why it is not automatically a qualifying application |
| --- | --- | --- |
| [WebRTC](https://www.w3.org/TR/webrtc/) | Peer sessions, ICE connectivity, optional TURN fallback | No intrinsic persistent dataset or peer discovery/signalling policy; applications must supply these |
| [mDNS / DNS-SD](https://www.rfc-editor.org/rfc/rfc6762) | LAN peer and service discovery | Temporary cache of advertised records, not durable application data |
| [tinc](https://www.tinc-vpn.org/) | Encrypted participant VPN mesh | Routes packets but does not itself replicate application content |
| [Nebula](https://nebula.defined.net/docs/) | Host-to-host encrypted overlay networking | Typical dynamic discovery uses lighthouse nodes; direct static peers alone do not establish stateful functionality |
| [LibreMesh](https://libremesh.org/) | Software for distributed wireless routers | Normally deployed on independently operated router hardware; not an ordinary end-user application |
| [Tor Onion Services](https://community.torproject.org/onion-services/) | Reachability through Tor network | Client/service depends on Tor routing and directories, not just two standalone clients |

## Inclusion boundary

These technologies can appear within a platform's ecosystem page or as implementation dependencies for qualifying applications. Optional transports and discovery do not certify the application itself, nor does having a local cache of DNS advertisements turn mDNS into a stateful user application.

Where a technology supports an isolated or peer-run mode, document the actual mode and dependencies rather than assuming the default internet deployment is server-optional.
