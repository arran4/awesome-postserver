# Contributing Guidelines

This repository maintains a curated list of software that enables multi-device syncing without reliance on central cloud servers. We are strict about what qualifies as "Post-Cloud", "True Serverless", or **"Post-Server"**.

## ℹ️ Definition of "Post-Server"

**Post-Server** means software operating without mandatory reliance on any third-party server or service.

*   **Relay servers are okay**, provided they do not lock the user in.
*   **Home servers are not okay** (typical Client-Server architecture).
*   **SMTP/POP3 counts** if any server can collect the mail and allow the user to retrieve it.

## 🛑 What DOES NOT Qualify

*   **Client-Server Architectures**: Even if the server is open-source and self-hostable (e.g., Nextcloud, Standard Notes, Bitwarden). If the primary sync mechanism is "Device A talks to Server, Device B talks to Server", it does not belong here.
*   **"Bring Your Own Sync" Apps**: Applications that simply save to a local file and rely on external tools (like Dropbox, Syncthing, or iCloud) to move that file around (e.g., KeePassXC, Obsidian, Logseq).
*   **Git Wrappers**: Applications whose primary claim to sync is simply auto-committing to a Git repository (e.g., Obsidian-git, Journal apps that just push to GitHub).
    *   *Exception*: Tools where the Git usage is "exceptional" (e.g., managing large binaries, handling partial checkouts in a unique P2P way, or complex merging logic independent of a central repo).
*   **Local-Only Apps**: Apps that have no networking or sync capabilities at all (e.g., a standard text editor).

## ✅ What Qualifies

*   **Peer-to-Peer (P2P) / Mesh**: Applications where devices communicate directly with each other (Client-to-Client) to synchronize data.
*   **Distributed Systems**: Software built on protocols like IPFS, Hypercore, BitTorrent, or custom gossip protocols.
*   **Base Synchronization Tools**: Tools that provide the *capability* to sync (merge logic, history, conflict resolution) but may be agnostic to the transport layer or designed for manual/disk transfer (e.g., Git itself, Windows Briefcase-style tools).
*   **Disk-Based Peer Sync**: Mechanisms where the software manages the synchronization logic between a source and a removable storage medium (acting as a peer).

## 📝 Rules for Adding Software

1.  **Verify the Sync Mechanism**: It must be P2P/Mesh by default or have a first-party mode for it.
2.  **Check Maturity**: Label as "Stable", "Beta", or "Alpha" accurately.
3.  **Categorize Correctly**: Use the existing categories (File Sync, Communication, etc.) or propose a new one if necessary.
