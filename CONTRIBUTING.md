# Contributing Guidelines

This repository maintains a curated list of software that enables multi-device syncing without reliance on central cloud servers. We are strict about what qualifies as "Post-Cloud" or "True Serverless".

## 🛑 What DOES NOT Qualify

*   **Client-Server Architectures**: Even if the server is open-source and self-hostable (e.g., Nextcloud, Standard Notes, Bitwarden). If the primary sync mechanism is "Device A talks to Server, Device B talks to Server", it does not belong here.
*   **"Bring Your Own Sync" Apps**: Applications that simply save to a local file and rely on external tools (like Dropbox, Syncthing, or iCloud) to move that file around (e.g., KeePassXC, Obsidian*, Logseq*).
    *   *Note: Some exceptions exist in the "Hybrid" section if they have significant community plugins that enable true P2P sync, but generally, we avoid them.*
*   **Local-Only Apps**: Apps that have no networking or sync capabilities at all (e.g., a standard text editor).

## ✅ What Qualifies

*   **Peer-to-Peer (P2P) / Mesh**: Applications where devices communicate directly with each other (Client-to-Client) to synchronize data.
*   **Distributed Systems**: Software built on protocols like IPFS, Hypercore, BitTorrent, or custom gossip protocols.
*   **Disk-Based Peer Sync**: Mechanisms like "Windows Briefcase" where the software manages the synchronization logic between a source and a removable storage medium (acting as a peer).

## 📝 Rules for Adding Software

1.  **Verify the Sync Mechanism**: It must be P2P/Mesh by default or have a first-party mode for it.
2.  **Check Maturity**: Label as "Stable", "Beta", or "Alpha" accurately.
3.  **Categorize Correctly**: Use the existing categories (File Sync, Communication, etc.) or propose a new one if necessary.
