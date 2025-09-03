# Qubes Architecture Overview

## Core Concepts
- **dom0**: Admin domain; manages GUI & hardware. Keep minimal; never browse here.
- **TemplateVMs**: Base images (e.g., Fedora/Ubuntu) used to spawn AppVMs.
- **AppVMs**: Daily-use VMs; data persists but software comes from TemplateVM.
- **Disposable VMs (DispVMs)**: Ephemeral VMs for handling untrusted files/links.
- **qrexec / inter‑VM policies**: Controlled communication between domains.

## Isolation Model
Each VM is a **separate security domain**; compromise in one domain does not imply compromise elsewhere.
Use color labels (red/yellow/green) to classify trust levels.

## Networking
NetVM → FirewallVM → AppVMs. Route Whonix through Tor for anonymity-critical tasks.
