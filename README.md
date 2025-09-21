# Wireshark Assignments — FTP, Telnet, RDesktop, DHCP (DORA)

## Overview
This repository contains Wireshark packet-capture assignments and analysis for common protocols and remote-access tools:
- **FTP** (file transfer protocol) captures and analysis  
- **Telnet** session captures and analysis  
- **RDesktop / Remote Desktop** traffic captures and notes (RDP analysis)  
- **DHCP DORA** (Discover, Offer, Request, Acknowledge) capture and explanation

All captures and tests were performed in a **controlled lab environment** using isolated virtual machines. These materials are for **educational purposes only**.

---

## Repository Structure
- `ftp/` — PCAPs, analysis notes, example commands, screenshots  
- `telnet/` — PCAPs, session transcripts, analysis notes  
- `rdesktop/` — RDP captures, connection logs, screenshots and explanation (if using rdesktop/tsclient)  
- `dhcp-dora/` — DHCP DORA capture(s) and step-by-step packet explanation  
- `reports/` — Consolidated findings and brief conclusions  
- `screenshots/` — Annotated screenshots from Wireshark

---

## Tools & Environment
- Wireshark — used to capture and analyze traffic  
- Test VMs: client and server on an isolated network (VirtualBox/VMware)  
- For RDP: `rdesktop` or native RDP client on the client VM connecting to an RDP server VM  
- For FTP/Telnet: simple server (vsftpd, inetutils-telnetd, or test services) on target VM

---

## Example Capture & Analysis Notes

### FTP
- Typical ports: `21` (control), data ports may be ephemeral or `20` (active mode).  
- Wireshark display filter to view FTP control traffic:  
