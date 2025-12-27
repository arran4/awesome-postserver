# Awesome Post-Cloud Post-NAS (True Serverless) Syncing

A curated list of software that enables multi-device syncing without reliance on central cloud servers or personal NAS setups. This is often referred to as "Local-First" or "Peer-to-Peer" (P2P) software.

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

### 💻 Code Collaboration

#### 🟢 Stable / Mature
*   **[Radicle](https://radicle.xyz/)** - A peer-to-peer, local-first code collaboration stack built on Git. It enables users to run their own nodes and collaborate without reliance on centralized forges like GitHub or GitLab.

### 🧠 Knowledge Management

### 💬 Communication

#### 🟢 Stable / Mature
*   **[Briar](https://briarproject.org/)** - A messaging app designed for activists and journalists. Syncs via Bluetooth, Wi-Fi, or Tor.

#### 🟡 Beta / In Development
*   **[Berty](https://berty.tech/)** - A secure, peer-to-peer messaging app using Bluetooth LE and mDNS. Currently in **Beta**.
*   **[BitChat](https://bitchat.free/)** - A decentralized peer-to-peer messaging application operating over Bluetooth mesh networks. No internet or servers required.
*   **[Scuttlebutt (Manyverse)](https://www.manyver.se/)** - A social network off the grid. Manyverse is a mobile app for the Scuttlebutt protocol. Currently in **Beta**.

---

## 🛠️ Hybrid / Capable (Centralized Default or Requires Configuration)

These applications are "Local-First". Some are centralized by default but offer P2P/Local modes (Hybrid), while others require specific configuration, plugins, or third-party tools (like Syncthing) to achieve serverless syncing.

### 📂 File Synchronization

#### 🟢 Stable / Mature
*   **[GoodSync](https://www.goodsync.com/)** - Primarily a backup/sync tool, but offers a specific P2P "GoodSync Connect" mode to sync directly between devices.

### 🧠 Knowledge Management

#### 🟢 Stable / Mature
*   **[Obsidian](https://obsidian.md/)** - A powerful knowledge base on top of a local folder of plain text Markdown files. Serverless sync is achieved via community plugins (e.g., `obsidian-git`, `remotely-save`) or external tools like Syncthing.
*   **[Joplin](https://joplinapp.org/)** - An open-source note-taking and to-do application. Supports synchronization via the file system (which can be synced via Syncthing).
*   **[TiddlyWiki](https://tiddlywiki.com/)** - A non-linear personal web notebook. It is a single HTML file that can be synced between devices using file synchronization tools.
    *   *Clients/Tools:* [TidGi](https://github.com/tiddly-gittly/TidGi-Desktop) (Desktop app with Git sync), [Tiddloid](https://github.com/donmor/Tiddloid) (Android).
*   **[Standard Notes](https://standardnotes.com/)** - A privacy-focused notes app. While it offers a centralized cloud by default, the server is open-source and can be [self-hosted](https://standardnotes.com/help/self-hosting/getting-started) for total control.
*   **[Notesnook](https://notesnook.com/)** - An end-to-end encrypted note-taking app. Offers a [self-hostable sync server](https://github.com/streetwriters/notesnook-sync-server).

#### 🟡 Beta / In Development
*   **[Bangle.io](https://bangle.io/)** - A web-only WYSIWYG note-taking app that saves notes locally in Markdown format. Sync can be achieved by syncing the local folder.
*   **[Anytype](https://anytype.io/)** - An "everything app" for notes, tasks, and knowledge management. Centralized by default (encrypted backup node), but supports local P2P syncing on the same network. Currently in **Open Beta**.
*   **[Logseq](https://logseq.com/)** - A privacy-first, open-source knowledge base. Default storage is local files; sync requires 3rd party tools or the beta sync service. Currently in **Beta**.
*   **[Affine](https://affine.pro/)** - A local-first, privacy-focused workspace combining docs, whiteboards, and databases. Self-hosting is required for serverless operation. Currently in **Beta**.
*   **[AppFlowy](https://www.appflowy.io/)** - An open-source alternative to Notion. Supports local offline mode; syncing requires self-hosting or cloud. Currently in **Beta**.

### 🔐 Password Management

#### 🟢 Stable / Mature
*   **[KeePassXC](https://keepassxc.org/)** - A cross-platform community-driven port of the Windows application “KeePass Password Safe”. It stores passwords in a local encrypted file, which can be synced across devices using file synchronization tools like Syncthing.

### 💰 Finance

#### 🟢 Stable / Mature
*   **[Actual Budget](https://actualbudget.com/)** - A local-first personal finance system. The core application is stable and open-source. Syncing typically requires a self-hosted relay server.
