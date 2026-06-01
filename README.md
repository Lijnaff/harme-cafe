# ☕ Harme Cafe

> Custom sales tracking, inventory automation, and business operations platform for a commercial cafe in Addis Ababa, Ethiopia.

## Overview

Harme Cafe is a full-stack business operation built from the ground up. This repo documents the custom software systems, network infrastructure, and brand assets that power the cafe's daily operations.

## What's Inside

### Sales & Inventory System
- Custom data scripting for daily sales tracking
- Automated inventory management with low-stock alerts
- Financial carry-over automation (daily → weekly → monthly reports)
- Reduced manual reporting errors by ~90%

### Network Infrastructure
- **pfSense** routing and firewall
- **OpenWrt** mesh WiFi across the premises
- **Dual-carrier 5G** for redundancy (primary + failover)
- **Captive portal** with voucher-based access control
- **Proxmox** host running Docker containers
- **NAS** with automated HD security camera backups

### Brand & Content
- Full brand identity design (logo, color palette, typography)
- Promotional video content (CapCut 4K, Premiere Pro)
- Social media assets (Photoshop, Illustrator)
- Menu design and print-ready layouts

## Tech Stack

| Domain | Tools |
|--------|-------|
| Data & Scripting | Python, Excel/Sheets automation |
| Networking | pfSense, OpenWrt, 5G, Captive Portal |
| Infrastructure | Proxmox, Docker, NAS |
| Design | Photoshop, Illustrator, CapCut 4K, Premiere Pro |

## Architecture

```
┌─────────────┐     ┌──────────────┐     ┌─────────────┐
│  POS Terminal│────▶│  Sales DB    │────▶│  Reports    │
│  (Frontend)  │     │  (Backend)   │     │  (Auto-gen) │
└─────────────┘     └──────────────┘     └─────────────┘
                           │
                    ┌──────▼──────┐
                    │  Inventory  │
                    │  Tracker    │
                    └─────────────┘

┌─────────────────────────────────────────────────────┐
│                 Network Layer                         │
│  pfSense ──▶ OpenWrt Mesh ──▶ Captive Portal        │
│  5G Carrier A ──▶ Failover ──▶ 5G Carrier B         │
│  Proxmox ──▶ Docker ──▶ NAS (Security Backup)       │
└─────────────────────────────────────────────────────┘
```

## Timeline

- **June 2024** — Founded, initial brand design
- **July 2024** — Network infrastructure deployed
- **August 2024** — Sales tracking system v1
- **October 2024** — Inventory automation live
- **January 2025** — Content production pipeline
- **Present** — Scaling to multi-location

## About the Founder

Built and maintained by **[Nafyad Fantaye](https://github.com/Lijnaff)** — Full-Stack Software Engineer & Digital Content Creator based in Addis Ababa, Ethiopia.

## License

This project documentation is MIT licensed. Business logic and brand assets are property of Harme Cafe.
