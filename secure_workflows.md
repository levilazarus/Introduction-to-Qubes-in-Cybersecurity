# Secure Workflows

## 1) Pentesting VM (AppVM)
- Based on a TemplateVM with security tools
- Tools: Metasploit, nmap, wfuzz, zaproxy
- Network: Isolate from personal AppVMs; no file sharing

## 2) Anonymous Browsing (Whonix)
- Route traffic through Tor (Whonix‑Gateway → Whonix‑Workstation)
- Use for OSINT and sensitive research

## 3) Everyday Work AppVM
- Office tasks; no pentesting tools
- Shared Clipboard strictly controlled (check Qubes settings)

## 4) Disposable VMs
- Open untrusted files/links
- Auto-destroy on close
