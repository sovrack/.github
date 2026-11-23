<div align="center">

# Sovrack

**The Sovereign Open-Core PaaS & Multi-Server Infrastructure Orchestration Platform**  
*Reclaim full sovereignty over your VPS, bare-metal servers, and application fleets from high-cost hyperscalers.*

[![License: Apache 2.0](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
[![CI / Quality Gates](https://img.shields.io/badge/CI-Passing_100%25-brightgreen.svg)](https://github.com/sovrack/sovrack/actions)
[![TypeScript 5.x](https://img.shields.io/badge/TypeScript-5.x-3178C6.svg)](https://www.typescriptlang.org/)
[![Go 1.22](https://img.shields.io/badge/Go-1.22-00ADD8.svg)](https://go.dev/)
[![Docker Ready](https://img.shields.io/badge/Docker-Production_Ready-2496ED.svg)](https://www.docker.com/)

[Website](https://sovrack.com) · [Documentation](https://docs.sovrack.com) · [Quickstart](https://docs.sovrack.com/getting-started/quickstart) · [Discord](https://discord.gg/sovrack)

</div>

---

## 🌟 Overview

Sovrack is a developer-first, self-hosted deployment platform engineered to combine the developer experience of modern cloud PaaS (Vercel, Supabase, Render) with complete infrastructure independence and zero vendor lock-in.

### Key Capabilities
- 🚀 **Automated Multi-Engine Builds** : Native Dockerfile generation and intelligent Nixpacks detection for Node.js, Go, Python, Rust, PHP, and Java.
- 🛡️ **Outbound Tunnel Agent in Go** : Connect and manage servers behind corporate firewalls, NAT routers, or private subnets without opening inbound SSH port 22.
- 📦 **1-Click Service Catalog** : Instant zero-configuration deployments of databases (PostgreSQL, MySQL, MongoDB), caches (Redis), message queues (RabbitMQ), object storage (MinIO), and tools (n8n, Uptime Kuma).
- 🌿 **Automated Preview Environments** : Dynamic ephemeral environments (`pr-42.preview.sovrack.com`) created automatically on GitHub/GitLab PRs and cleaned up on merge.
- 🔒 **Wildcard SSL via DNS-01** : Automated Let's Encrypt Wildcard certificates (`*.yourdomain.com`) through Cloudflare, OVH, and DigitalOcean APIs.
- 💾 **Continuous WAL Streaming & PITR** : PostgreSQL disaster recovery with streaming WAL to S3 / Cloudflare R2 and Point-In-Time recovery to the exact second.

---

## 🏛️ Ecosystem Repositories

| Repository | Description | Tech Stack |
| :--- | :--- | :--- |
| [**sovrack/sovrack**](https://github.com/sovrack/sovrack) | Core Monorepo : NestJS 11 Control Plane, Next.js 15 Web Console & Traefik/Nginx Infra | TypeScript, NestJS, Next.js, Prisma, Docker |
| [**sovrack/agent**](https://github.com/sovrack/agent) | Lightweight Outbound Tunnel Agent (<15MB RAM) for firewalled & NAT servers | Go 1.22, WebSockets, gopsutil |
| [**sovrack/cli**](https://github.com/sovrack/cli) | Official Command-Line Interface for terminal automation and remote deploy | Node.js, TypeScript, Commander |
| [**sovrack/sdk**](https://github.com/sovrack/sdk) | Typed TypeScript / Node.js SDK for programmatic platform control | TypeScript, Axios |
| [**sovrack/templates**](https://github.com/sovrack/templates) | Verified 1-Click Service Stacks Catalogue & Manifests | JSON, Docker Specifications |
| [**sovrack/installer**](https://github.com/sovrack/installer) | Automated 1-liner host provisioning and installation script | POSIX Bash |
| [**sovrack/docs**](https://github.com/sovrack/docs) | Architecture guides, runbooks, and comprehensive API documentation | Markdown |

---

## ⚡ Quickstart

Install Sovrack on any clean Ubuntu 22.04+ or Debian 12+ VPS with one command :

```bash
curl -fsSL https://raw.githubusercontent.com/sovrack/installer/main/install.sh | sudo bash
```

Once installed, open your browser at `http://<YOUR_SERVER_IP>:3000` to set up your primary administrator account.

---

## 📜 Open-Core Licensing

Sovrack is built on an **Open-Core** model :
- The core platform, agents, CLI, and SDK are licensed under the permissive **[Apache License 2.0](https://github.com/sovrack/sovrack/blob/main/LICENSE)**.
- Enterprise extensions (SAML/SSO, advanced audit vaults, air-gapped compliance) are isolated under `/ee` with source-available commercial terms.

---

<div align="center">
<sub>Built with passion for infrastructure sovereignty. &copy; 2026 Sovrack.</sub>
</div>
