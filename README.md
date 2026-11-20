# Awesome Post-Server

Software for sharing, communication and persistent data **without requiring a dedicated server**. Participating devices can connect directly, share state or forward information for one another; fixed home servers and mandatory always-on relays are outside the intended scope.

The main list prioritizes *usable, stateful applications*. For wider protocol ecosystems and accessory software, we link to existing maintained indexes rather than copying them into this catalog. “Local-first”, “federated” or “decentralized” does not automatically mean server-optional.

> **Catalog review in progress:** Some older entries and open PRs predate this stricter definition. Treat their placement as provisional until reassessed.

## 🌐 Fully Distributed / P2P by Default

These applications are designed from the ground up to be serverless and distributed. Syncing is their native mode of operation using P2P protocols without reliance on a central server.

### 📂 File Synchronization

#### 🟢 Stable / Mature
*   **[Syncthing](https://syncthing.net/)** - A continuous file synchronization program. It synchronizes files between two or more computers in real time, safely protected from prying eyes. Open Source and uses the Block Exchange Protocol.
    *   *Clients:* [SyncTrayzor](https://github.com/canton7/SyncTrayzor) (Windows), [Mobius Sync](https://apps.apple.com/us/app/mobius-sync/id1539193212) (iOS), [Syncthing-Fork](https://github.com/Catfriend1/syncthing-android) (Android).
*   **[Resilio Sync](https://www.resilio.com/individuals/)** - Formerly BitTorrent Sync. A proprietary P2P file synchronization tool that is fast and reliable, using the BitTorrent protocol.

#### 🟡 Beta / In Development
*   **[Spacedrive](https://www.spacedrive.com/)** - An open source cross-platform file explorer, powered by a virtual distributed filesystem (VDFS). Currently in **Alpha**.
*   **[Peergos](https://peergos.org/)** - A P2P, private, and end-to-end encrypted social storage platform. Aims to replace Google Drive/Photos.
*   **[IPFS Desktop](https://docs.ipfs.tech/install/ipfs-desktop/)** - A desktop client for the InterPlanetary File System. While the protocol is established, the desktop user experience is still evolving.

### 🧱 Base Synchronization Tools / Protocols

These tools provide the core capabilities for peer-to-peer synchronization (merging, history, state reconciliation) but may require manual transport (disk) or a separate network layer to function.

*   **[Git](https://git-scm.com/)** - A distributed version control system. It enables P2P syncing of code and text via various transports (SSH, HTTP, Bundle files) and handles complex merging and history.
*   **[git-annex](https://git-annex.branchable.com/)** - Manages files with Git, without checking the file contents into Git. It allows managing files with git, yet looking up file contents in a distributed way. Includes a [P2P protocol](https://git-annex.branchable.com/git-annex-p2p/) for connecting repositories directly.
*   **[Unison](https://github.com/bcpierce00/unison)** - A file-synchronization tool for OSX, Unix, and Windows. It allows two replicas of a collection of files and directories to be stored on different hosts (or different disks on the same host), modified separately, and then brought up to date by propagating the changes in each replica to the other.

### 💻 Code Collaboration

#### 🟢 Stable / Mature
*   **[Radicle](https://radicle.xyz/)** - A peer-to-peer, local-first code collaboration stack built on Git. It enables users to run their own nodes and collaborate without reliance on centralized forges like GitHub or GitLab.

### 🧠 Knowledge Management

### 📢 Social Networks & Feeds

#### 🟡 Beta / In Development
*   **[Scuttlebutt (Manyverse)](https://www.manyver.se/)** - A peer-to-peer social network protocol. Users store their own content and sync directly (Wi-Fi, Bluetooth, or Pubs). Manyverse is a popular client.

### 💬 Communication

#### 🟢 Stable / Mature
*   **[Briar](https://briarproject.org/)** - A messaging app designed for activists and journalists. Syncs via Bluetooth, Wi-Fi, or Tor.
*   **[I2P-Bote](https://github.com/i2p/i2p.i2p-bote)** - A fully serverless, end-to-end encrypted email system operating within the I2P network. It stores emails in a distributed hash table (DHT) ensuring anonymity and resilience.
*   **[Jami](https://jami.net/)** - A GNU project. Peer-to-peer audio/video calls, messaging, and file transfer. Uses a distributed hash table (DHT) for user discovery.
*   **[Session](https://getsession.org/)** - A private messenger that routes messages through an onion-routing network (Oxen) to strip metadata. No phone numbers required; uses Account IDs. All messages are end-to-end encrypted and stored on decentralized nodes.
*   **[SimpleX Chat](https://simplex.chat/)** - An open-source messenger with no user identifiers (no phone numbers or usernames). It uses transient relay servers (queues) to pass encrypted messages, ensuring no metadata about who contacts whom is exposed. Fully decentralized and independent.

#### 🟡 Beta / In Development
*   **[Cwtch](https://cwtch.im/)** - A decentralized, metadata-resistant group chat platform. Users can host their own "safe spaces" (servers) for group conversations. All communication is routed via Tor v3 onion services for anonymity.
*   **[Berty](https://berty.tech/)** - A secure, peer-to-peer messaging app using Bluetooth LE and mDNS. Currently in **Beta**.
*   **[BitChat](https://bitchat.free/)** - A decentralized peer-to-peer messaging application operating over Bluetooth mesh networks. No internet or servers required.
*   **[Tox](https://tox.chat/)** - A P2P instant-messaging and video-calling protocol. Uses a distributed hash table (DHT) and provides end-to-end encryption.
*   **[Keet](https://keet.io/)** - A P2P chat, video, and file sharing app built on the [Holepunch](https://holepunch.to/) platform. It uses a distributed database (Hypercore) to sync data directly between peers.
*   **[RetroShare](https://retroshare.cc/)** - A decentralized communication platform for secure chat, file sharing, and mail. It builds a Friend-to-Friend (F2F) network.
*   **[Cabal](https://cabal.chat/)** - An experimental P2P community chat platform. Chats are stored locally and synced directly between peers.

#### 🔴 Legacy / Historical
*   **[Bitmessage](https://github.com/Bitmessage/PyBitmessage)** - An encrypted, anonymous P2P messaging protocol. Messages are replicated to all nodes (flooding) for anonymity. *Note: No longer in active development.*

---

## 🛠️ Hybrid / Capable (under architectural review)

> **Provisional entries:** Local-first storage, self-hosting or external synchronization is not sufficient under the stricter server-optional definition. These historical entries remain visible while each application's native peer mode, persistent state and mandatory service dependencies are checked. They are **not** automatically recommended or eligible for the main list.

### 📂 File Synchronization

#### 🟢 Stable / Mature
*   **[GoodSync](https://www.goodsync.com/)** - Primarily a backup/sync tool, but offers a specific P2P "GoodSync Connect" mode to sync directly between devices.

### 🧠 Knowledge Management

#### 🟡 Beta / In Development
*   **[Anytype](https://anytype.io/)** - An "everything app" for notes, tasks, and knowledge management. Centralized by default (encrypted backup node), but supports local P2P syncing on the same network. Currently in **Open Beta**.
*   **[Logseq](https://logseq.com/)** - A privacy-first, open-source knowledge base. Default storage is local files; sync requires 3rd party tools or the beta sync service. Currently in **Beta**.
*   **[Affine](https://affine.pro/)** - A local-first, privacy-focused workspace combining docs, whiteboards, and databases. Self-hosting is required for serverless operation. Currently in **Beta**.
*   **[AppFlowy](https://www.appflowy.io/)** - An open-source alternative to Notion. Supports local offline mode; syncing requires self-hosting or cloud. Currently in **Beta**.

### 💰 Finance

#### 🟢 Stable / Mature
*   **[Actual Budget](https://actualbudget.com/)** - A local-first personal finance system. The core application is stable and open-source. Syncing typically requires a self-hosted relay server.

## Related ecosystem indexes (not Post-Server endorsements)

These broader collections include protocols, libraries and applications that **have not necessarily passed** our two-device, server-optional and persistent-state criteria. We refer to the original maintainers instead of reproducing their lists.

- **[Delay-/disruption-tolerant networking — Awesome DTN](https://github.com/dtn7/awesome-dtn):** BPv7 uses bundles that can be stored and forwarded when devices reconnect. The upstream list covers implementations and applications; BPv7 itself is not a finished end-user application.
- **[IPFS — Awesome IPFS](https://github.com/ipfs/awesome-ipfs):** Network implementations, publishing applications and accessories, including gateway-only tools that may not qualify here.
- **[libp2p — Awesome libp2p](https://github.com/libp2p/awesome-libp2p):** Discovery, routing, transport and software built with those primitives; these alone do not make an application stateful or server-optional.
- **[Reticulum — Awesome Reticulum](https://github.com/lorien/awesome-reticulum):** Nodes, messaging applications, radio adapters and accessories whose required infrastructure must be evaluated individually.

If a useful project is missing from one of these indexes, prefer contributing it **upstream**. If the project also independently satisfies our stricter Post-Server definition, list it in the appropriate application category here with evidence, rather than creating a parallel ecosystem directory.

