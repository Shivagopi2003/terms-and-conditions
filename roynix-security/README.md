# 🛡️ Roynix Security (Roynix Shield)

> **Next-Generation Discord Security, Anti-Nuke, Anti-Raid & Server Defense Engine.**

[![Discord Support](https://img.shields.io/badge/Discord-Support%20Server-5865F2?logo=discord&logoColor=white)](https://discord.gg/XA4VZMYsbP)
[![Developer](https://img.shields.io/badge/Developer-Shiva-blue)](https://discord.gg/XA4VZMYsbP)
[![Terms of Service](https://img.shields.io/badge/Legal-Terms%20of%20Service-green)](./terms-and-conditions/README.md)
[![Privacy Policy](https://img.shields.io/badge/Legal-Privacy%20Policy-orange)](./privacy-policy/README.md)

---

## 📌 Bot Overview

**Roynix Security** (also known as **Roynix Shield**) is an enterprise-grade Discord security bot engineered to defend communities from malicious nuke attacks, compromised administrator credentials, automated bot raids, unauthorized permission tampering, and fraudulent content.

Designed with an ultra-low-latency event pipeline, Roynix Security processes raw Discord Gateway dispatches and audit log events within milliseconds, coordinating instant automated mitigation, role revocation, and server blueprint restoration.

* **Application Name:** Roynix Security / Roynix Shield
* **Developer & Lead Engineer:** Shiva (`788970167907778562`)
* **Official Support Server:** [https://discord.gg/XA4VZMYsbP](https://discord.gg/XA4VZMYsbP)
* **Official Repository:** [https://github.com/shivaa1906/TERMS-AND-CONDITIONS](https://github.com/shivaa1906/TERMS-AND-CONDITIONS)
* **Contact Email:** [shivaa1906@gmail.com](mailto:shivaa1906@gmail.com)

---

## ⚡ Core Protection Modules

Roynix Security features a comprehensive suite of independent, configurable defense modules:

### 1. Bot & Identity Defense
* **Verified Bot Protection:** Evaluates Discord's authoritative REST User Flags (`VerifiedBot = 65536`) to identify unverified bots upon joining. Supports configurable Audit-Only observation and automated banning of unverified bots.
* **Admin Secure:** Detects unauthorized bot additions and immediately strips administrative permissions and roles from the responsible administrator, neutralizing rogue staff attacks.
* **Anti-Bot:** Enforces inviter attribution and blocks unauthorized bot invites unless explicitly whitelisted or authorized by the server owner.
* **Zero-Trust Quarantine:** Quarantines newly invited bots and prevents unapproved automated bots from gaining dangerous guild permissions.

### 2. Server Structure & Asset Defense
* **Anti-Channel Protection:** Intercepts unauthorized channel deletion, creation, and modification.
* **Channel Overwrite Protection:** Detects and reverts unauthorized dangerous permission overwrite additions on protected channels.
* **Anti-Role Protection:** Prevents unauthorized role deletion, role creation, and role edits.
* **Role Position Protection:** Reverts unauthorized role hierarchy escalation and position tampering.
* **Permission Escalation:** Instantly revokes administrative or dangerous permission grants added to existing roles.
* **Blueprint Auto-Recovery:** Automatically reconstructs maliciously deleted channels and roles (including permissions, positions, and channel settings) from cached blueprints.

### 3. Moderation & Raid Defense
* **Anti-Ban & Anti-Kick:** Punishes untrusted actors who ban or kick server members and restores victims via idempotent unbanning.
* **Anti-Unban:** Blocks unauthorized removal of server bans.
* **Anti-Prune:** Detects and halts unauthorized mass member pruning.
* **Join Raid Protection:** Analyzes join burst velocity and triggers server-wide protective measures during wave raids.
* **Circuit Breaker:** Automated emergency server lockdown that engages during high-velocity attacks to isolate the guild.

### 4. Content & Webhook Security
* **Anti-Webhook:** Automatically deletes unauthorized webhooks created by non-exempt members.
* **Integration Protection:** Monitors external application connections and removes unauthorized integrations.
* **Anti-Emoji & Anti-Sticker:** Protects server emojis and stickers from unauthorized mass deletion or replacement.
* **Phishing & Scam Filter:** Real-time in-memory message screening against known phishing domains, typo-squatted URLs, and fake Discord Nitro lure patterns.
* **Attachment Screening:** Blocks and removes dangerous executable attachments (`.exe`, `.bat`, `.vbs`, `.sh`, `.py`).
* **Anti-Spam Rate Limiter:** Per-user token bucket rate limiting preventing rapid copy-paste message floods.

---

## 🔐 Permission Hierarchy & Best Practices

To enable Roynix Security to protect your server effectively:

1. **Role Position:** In Server Settings $\to$ Roles, place the **Roynix Security** role as high in the role hierarchy as possible (directly below the Server Owner role).
2. **Discord Hierarchy Rule:** Discord platform rules strictly prevent any bot from modifying members or roles positioned higher than or equal to the bot's own highest role.
3. **Recommended Permissions:**
   * `Administrator` (Recommended for full protection suite), or:
   * `View Audit Log`
   * `Manage Roles`
   * `Manage Channels`
   * `Ban Members`
   * `Kick Members`
   * `Manage Webhooks`
   * `Moderate Members` (Timeout)

---

## 📖 Commands & Configuration

Roynix Security supports both Slash (`/`) and Prefix (`!`) commands:

| Command | Type | Description |
| :--- | :--- | :--- |
| `/antinuke enable` | Admin | Enable the Anti-Nuke system with guided setup. |
| `/antinuke disable` | Owner | Temporarily disable the Anti-Nuke protection. |
| `/antinuke config` | Admin | View current server protection settings and module states. |
| `/antinuke modules` | Admin | Toggle individual security modules on or off. |
| `/antinuke whitelist` | Owner | Add or remove trusted members and bots from the whitelist. |
| `/antinuke extraowner` | Owner | Assign extra owners with full security management privileges. |
| `/antinuke logs` | Admin | Configure the designated security incident logs channel. |
| `/stats` | Public | Display bot uptime, gateway latency, and protection metrics. |
| `/help` | Public | View the interactive command guide and documentation. |

---

## 📄 Legal & Compliance Documentation

Roynix Security complies with Discord's Developer Terms of Service, Discord Community Guidelines, and global data privacy standards:

* 📜 **[Terms and Conditions (Terms of Service)](./terms-and-conditions/README.md)** — Terms governing the use of Roynix Security.
* 🔒 **[Privacy Policy](./privacy-policy/README.md)** — How user and server data is collected, processed, and safeguarded.

---

## 💬 Support & Inquiries

Need assistance setting up Roynix Security, reporting a security incident, or requesting data deletion?
* **Discord Support Server:** [https://discord.gg/XA4VZMYsbP](https://discord.gg/XA4VZMYsbP)
* **Lead Developer:** Shiva (`788970167907778562`)
* **Email:** [shivaa1906@gmail.com](mailto:shivaa1906@gmail.com)
