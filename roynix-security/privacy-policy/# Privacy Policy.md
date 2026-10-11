# Privacy Policy — Roynix Security

**Effective Date:** October 11, 2026  
**Last Updated:** October 11, 2026  
**Application Name:** Roynix Security (Roynix Shield)  
**Developer / Owner:** Shiva (`788970167907778562`)  
**Official Support Server:** [https://discord.gg/XA4VZMYsbP](https://discord.gg/XA4VZMYsbP)  

---

## 1. Introduction & Commitment to Privacy

Your privacy and data security are core priorities for **Roynix Security** ("the Bot", "Service", "We", "Us", or "Our"). This Privacy Policy explains what information we collect, how it is used, how it is stored, and your rights concerning your data when you add, configure, or interact with Roynix Security in your Discord server.

We adhere strictly to the principle of **data minimization**: we only collect and process data that is strictly necessary to operate, maintain, and deliver our automated security and server protection services.

---

## 2. Information We Collect

### A. Discord Identifiers (Metadata)
To authenticate users and enforce guild-specific security policies, we process:
* **Guild (Server) IDs:** To associate configurations, logs, and defense states with specific servers.
* **User IDs:** To verify server ownership, enforce whitelists, track extra owners, record incident executors, and apply authorized punishments.
* **Role & Channel IDs:** To monitor changes, protect critical server assets, and maintain channel blueprints.

### B. Server Configuration & Security Settings
When administrators configure Roynix Security, we store:
* Enabled/disabled security modules (e.g., Anti-Bot, Anti-Channel Delete, Admin Secure, Verified Bot Protection).
* Configured punishment preferences (`ban`, `kick`, `timeout`).
* Whitelisted user and bot IDs.
* Logging channel IDs and custom prefix configurations.

### C. Server Blueprints & Restoration Snapshots
To enable instant recovery when channels or roles are maliciously deleted:
* **Channel Blueprints:** Channel names, types, topics, parent categories, and permission overwrites.
* **Role Blueprints:** Role names, colors, hoist status, position metadata, and permission bitfields.
* *Note:* Server blueprints strictly contain server structural metadata; they do not contain user messages or chat histories.

### D. Audit Log & Incident Telemetry
When a security event or raid is detected:
* Timestamps of detected events.
* Target IDs (e.g., affected channel, role, or member).
* Executor IDs (attribution resolved through Discord audit logs).
* Action outcomes (e.g., `Bot Banned`, `Admin Roles Revoked`, `Channel Restored`).

### E. Transient Message & Content Telemetry
* Messages sent in protected channels are inspected **in-memory in real time** solely to detect phishing URLs, fraudulent scam patterns, executable malware attachments, and high-frequency message flooding.
* **Message contents are NEVER permanently stored in our databases**, never logged to disk, and never shared or analyzed for behavioral profiling.

---

## 3. How We Use Collected Information

The information collected is used exclusively for the following operational purposes:
1. **Automated Server Defense:** Detecting and neutralizing unauthorized bot additions, channel deletions, mass kicks, or permission escalation.
2. **Access Control:** Verifying whether a command author is the guild owner or an authorized extra owner.
3. **Recovery & Reconstruction:** Restoring deleted channels and roles to their pre-incident state using cached blueprints.
4. **Audit Logging & Notifications:** Dispatching security alert embeds to your designated logging channels.
5. **System Stability & Health:** Diagnosing execution latency, rate limit pressure, and internal errors.

---

## 4. Data Sharing & Third Parties

* **No Data Sales:** We do **NOT** sell, rent, trade, monetize, or license your data to third parties under any circumstances.
* **No Advertising:** We do not use your data for advertising, marketing, or behavioral tracking.
* **Third-Party Disclosures:** Data is never shared with third parties, except where required by law, legal process, or to comply with valid legal requests from law enforcement authorities.

---

## 5. Data Storage, Security & Retention

1. **Storage Infrastructure:** Data is stored in secure, password-protected local databases (SQLite / FastDB) hosted on private, hardened server infrastructure.
2. **Access Restrictions:** Access to the database is restricted strictly to the primary bot developer and core service processes.
3. **Retention Periods:**
   * **In-Memory Caches & Deduplication:** Flushed and evicted automatically every 8 to 60 seconds.
   * **Server Configuration Data:** Retained for as long as Roynix Security remains active in your Discord server.
   * **Incident Logs:** Retained in rotating bounded histories for auditing and threat scoring.

---

## 6. Data Deletion & Your Rights

You have the following rights regarding your data:
1. **Right to Opt-Out:** You can stop all data collection at any time simply by removing or banning Roynix Security from your Discord server.
2. **Right to Data Deletion:**
   * Server owners may request complete and permanent deletion of their server's configuration, incident logs, and blueprints at any time.
   * To request data deletion, join our [Official Support Server](https://discord.gg/XA4VZMYsbP) or contact `shivaa1906@gmail.com` with your Server ID. Your request will be fulfilled within **7 business days**.

---

## 7. Children's Privacy

Roynix Security complies with the Children's Online Privacy Protection Act (COPPA) and Discord's Terms of Service. We do not knowingly collect or maintain information from children under the age of 13. If you become aware that a child under 13 has provided personal data, please contact us immediately to have the data removed.

---

## 8. Changes to this Privacy Policy

We may update this Privacy Policy from time to time to reflect changes in our security mechanisms, legal obligations, or Discord platform requirements. Any updates will be reflected with a revised "Last Updated" date at the top of this document. Continued use of Roynix Security after updates constitute acceptance of the revised policy.

---

## 9. Contact Information

If you have questions, feedback, or data privacy requests, please reach out to us:
* **Official Discord Support Server:** [https://discord.gg/XA4VZMYsbP](https://discord.gg/XA4VZMYsbP)
* **Lead Developer Discord:** Shiva (`788970167907778562`)
* **Email:** [shivaa1906@gmail.com](mailto:shivaa1906@gmail.com)
* **Official Repository:** [https://github.com/shivaa1906/TERMS-AND-CONDITIONS](https://github.com/shivaa1906/TERMS-AND-CONDITIONS)
