# Metasploitable 2 — Network Reconnaissance & Exploitation Lab

A hands-on, self-directed cybersecurity lab project: building an isolated virtual network, scanning and enumerating a deliberately vulnerable target, and exploiting a known service backdoor to obtain root access — fully documented from first command to final flag.

## Overview

This project uses **Metasploitable 2**, an intentionally vulnerable Linux VM built for security training, as the target. All work was performed inside a private, isolated VirtualBox lab network with no connection to the internet on the target machine.

## What I Did

- Built and networked an isolated lab (Kali Linux attacker VM + Metasploitable 2 target VM) using VirtualBox Host-only networking
- Performed host discovery and service enumeration with **Nmap**
- Manually verified findings with `netcat` and direct FTP login
- Identified a known, publicly documented backdoor (CVE-adjacent 2011 vsftpd 2.3.4 supply-chain compromise)
- Used **Metasploit** to trigger the backdoor and obtain a root-level shell on the target
- Documented the entire process in a structured lab report

## Tools Used

Kali Linux, VirtualBox, Nmap, Netcat, Metasploit Framework

## Repository Structure 

├── README.md
├── reports/
│ └── Lab report (full write-up: methodology, commands, findings, analysis)
└── Evidence/
└── nmap_scan.txt — raw Nmap scan output

## Full Write-Up

See [`reports/`](./reports) for the complete report, including reconnaissance methodology, enumeration findings, the exploitation walkthrough, and lessons learned.

## Disclaimer

This project was conducted entirely within a private, isolated lab environment against a machine intentionally built for security training. No real-world, third-party, or production systems were involved at any point.
