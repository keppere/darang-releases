# Darang

**A fast, cross-platform SQL IDE and database workspace.** Query PostgreSQL, MySQL, SQLite, Cloudflare D1 and Elasticsearch, and manage your SSH hosts, all from one window.

[![Latest release](https://img.shields.io/github/v/release/keppere/darang-releases?label=latest)](https://github.com/keppere/darang-releases/releases/latest)
![Platforms](https://img.shields.io/badge/platforms-Windows%20%7C%20macOS%20%7C%20Linux-blue)

This repository hosts the **official installers and release notes**. The app source is private.

---

## Download

Grab the build for your system from the [latest release](https://github.com/keppere/darang-releases/releases/latest).

| Platform    | File                                          | Architecture          |
| ----------- | --------------------------------------------- | --------------------- |
| **Windows** | `Darang-Setup-X.Y.Z.exe`                      | x64                   |
| **macOS**   | `Darang-X.Y.Z-arm64.dmg` / `Darang-X.Y.Z.dmg` | Apple Silicon / Intel |
| **Linux**   | `Darang-X.Y.Z.AppImage`, `.deb`, `.rpm`       | x64                   |

Darang checks for updates on its own. When one is available, an **Update** badge appears in the status bar. Nothing downloads until you click it.

---

## What you get

### Databases
- **PostgreSQL, MySQL, SQLite, Cloudflare D1 and Elasticsearch** in one client, with full schema browsing, table, view and trigger editors, and export.
- **Multiple live connections at once.** Each keeps its own tabs, draft queries and editor state.
- **Elasticsearch** in SQL, DSL and ES|QL modes, with a Kibana DevTools-style console.
- **Cloudflare D1** over the REST API, with schema introspection and atomic script batches.
- Dialect-aware editing in the results grid, with identifiers quoted correctly.

### Editor and workflow
- A Monaco-based SQL editor (the engine behind VS Code), with a built-in formatter and query history.
- Notebooks and dashboards: mix SQL, notes and charts in one document.
- Visual schema diagrams.
- A launcher (`Alt+L`) for quick search, schema, explorer and settings.
- Vertical tabs grouped by connection, so open work stays organised by server and database.

### SSH, built in
- Integrated terminal sessions, an SFTP file explorer and live CPU and memory monitoring.
- Jump hosts, local and remote port forwarding, and SSH tunnels for database connections.

### Security
- Credentials are sealed locally with **AES-256-GCM** under a master key that never leaves your machine.
- Master key derivation uses salted scrypt.
- Production connections get confirmation gates before destructive actions.
- Optional **Darang Cloud** sync for connections, projects and documents.

---

## Install

### Windows
1. Download `Darang-Setup-X.Y.Z.exe` and run it.
2. Follow the installer. Darang launches when it finishes.

### macOS
1. Download the `.dmg` that matches your Mac: `arm64` for Apple Silicon, the plain one for Intel.
2. Open it and drag **Darang** into **Applications**.

### Linux
**AppImage**
```bash
chmod +x Darang-X.Y.Z.AppImage
./Darang-X.Y.Z.AppImage
```

**Debian / Ubuntu**
```bash
sudo apt install ./darang_X.Y.Z_amd64.deb
```

**Fedora / RHEL**
```bash
sudo dnf install ./darang-X.Y.Z.x86_64.rpm
```

---

## Feedback and support

- Found a bug or want a feature? [Open an issue](https://github.com/keppere/darang-releases/issues).
- See what changed in each version on the [Releases page](https://github.com/keppere/darang-releases/releases).
