<div align="center">

# Sovrack

**The Open-Core Deployment & Orchestration Platform**  
*Deploy Docker applications and containers directly on your own Ubuntu servers with zero vendor lock-in.*

[![Website](https://img.shields.io/badge/Website-sovrack.com-2563EB?style=flat-square)](https://sovrack.com)
[![Documentation](https://img.shields.io/badge/Docs-docs.sovrack.com-2563EB?style=flat-square)](https://docs.sovrack.com)
[![Discord](https://img.shields.io/badge/Discord-Join%20Community-5865F2?style=flat-square&logo=discord&logoColor=white)](https://discord.gg/sovrack)
[![Twitter](https://img.shields.io/badge/Twitter-@sovrack-000000?style=flat-square&logo=x&logoColor=white)](https://x.com/sovrack)
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg?style=flat-square)](LICENSE)

</div>

---

## What is Sovrack?

**Sovrack** is a modern, developer-centric PaaS that turns your own VPS or dedicated servers into a fully automated deployment platform. It gives you the convenience and developer experience of managed cloud platforms (like Vercel or Heroku) with the sovereignty, cost efficiency, and performance of bare-metal and self-hosted infrastructure.

### ✨ Key Capabilities

- 🚀 **Agentless SSH Architecture**: No heavy background agents required on target servers. Sovrack connects via encrypted SSH key tunnels and manages Docker natively.
- 📦 **Universal Build Engine (Nixpacks & Docker)**: Automatic runtime detection for Node.js, Python, Go, Rust, PHP, Java, Static sites, or custom Dockerfiles.
- 🔄 **Git-Powered CI/CD**: One-click integration with GitHub and GitLab. Push to your branch and trigger automated releases with instant zero-downtime rolling deploys.
- 🔒 **Automated HTTPS & Routing**: Built-in dynamic reverse proxy (Nginx & Traefik) with automatic TLS certificate provisioning via Let's Encrypt.
- 📊 **Unified Observability**: Live server health metrics (CPU, RAM, Disk, Load), container logs, and monitoring out of the box.
- 🖥️ **Web SSH Terminal**: Direct root access to your servers from your browser with full security audit logging.

---

## 🏛️ Ecosystem Repositories

| Repository | Description | Status |
| :--- | :--- | :--- |
| [**sovrack/sovrack**](https://github.com/sovrack/sovrack) | The core mono-repository containing the NestJS backend API, Next.js web console, and orchestration workers. | Active |
| [**sovrack/cli**](https://github.com/sovrack/cli) | Official command-line interface to deploy and manage services directly from your terminal. | Active |
| [**sovrack/docs**](https://github.com/sovrack/docs) | Official developer documentation, deployment guides, tutorials, and API reference. | Active |
| [**sovrack/.github**](https://github.com/sovrack/.github) | Organization profile, community health files, issue templates, and contribution workflows. | Active |

---

## ⚡ Quickstart

Deploy Sovrack on an Ubuntu 22.04 / 24.04 LTS server in less than 2 minutes:

```bash
curl -fsSL https://get.sovrack.com | bash
```

Once installed, open your browser at `http://your-server-ip:3000` to complete the initial setup and attach your first VPS.

---

## 🌐 Connect with the Community

- **Official Website**: [sovrack.com](https://sovrack.com)
- **Documentation**: [docs.sovrack.com](https://docs.sovrack.com)
- **Community Discord**: [Join our Discord](https://discord.gg/sovrack)
- **X (Twitter)**: [@sovrack](https://x.com/sovrack)
- **LinkedIn**: [Sovrack](https://linkedin.com/company/sovrack)

---

<div align="center">
  <sub>Built with ❤️ by the Sovrack team and community contributors worldwide.</sub>
</div>
