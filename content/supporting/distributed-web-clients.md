---
title: "Distributed-web browser clients"
description: "Clients that navigate peer content, with publishing/serving evaluated separately."
---

# Distributed-web browsers and accessories

**Assessment:** Supporting applications pending a peer-hosting demonstration.  
**Maturity:** Varies by project. **Reviewed:** 2026-11-19.

Browsing content over IPFS or Hypercore is useful, but it does not automatically mean the *browser* is a server-optional publishing application. A client that only fetches content should be linked under the corresponding protocol instead of promoted as a standalone post-server solution.

- [Agregore](https://github.com/AgregoreWeb/agregore-browser): browser for peer-to-peer protocols. Examine whether an ordinary installation can **publish and serve** persisted content without a separately run node.
- [PeerSky](https://github.com/p2plabsxyz/peersky-browser): experimental P2P browser. Verify its implemented protocol handlers and any integrated hosting/seeding modes.
- [Ceno](https://ceno.app/): web access and caching over a sharing network, including potential dependencies on injector services for uncached origins. Distinguish shared cached content from independent peer publishing.
- [IPFS Desktop](https://docs.ipfs.tech/install/ipfs-desktop/): companion GUI for an IPFS node, already included in the main README; needs a mode-specific audit of whether the node genuinely serves/pins content.

## Graduation criteria

Demonstrate two participant devices where one can create, sign, store, announce and serve content using the proposed product, and the other can retrieve/replicate it without a third mandatory storage provider, index or gateway. Distinguish browser-integrated serving from a separately installed external synchronization application.

Until verified, retain references here instead of describing each browser as a stand-alone qualifying application.
