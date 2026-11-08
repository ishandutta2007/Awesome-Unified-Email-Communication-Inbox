# Awesome-Unified-Email-Communication-Inbox

# Awesome Unified Email & Communication Inbox

> A curated list of top Unified Email and Communication Inbox platforms — both SaaS/Hosted commercial solutions and open-source alternatives for collaborative shared inboxes, team email management, and omnichannel communication.  
> 🌟 Star this repo if you find it useful! 🌟

---

## 📋 Table of Contents

- [SaaS / Hosted Platforms](#-saas--hosted-platforms)
  - [Front](#front)
  - [Missive](#missive)
  - [Hiver](#hiver)
  - [Superhuman](#superhuman)
  - [Spark Mail](#spark-mail)
  - [Help Scout](#help-scout)
  - [Gmelius](#gmelius)
  - [Crisp](#crisp)
- [Open-Source Software](#-open-source-software)
  - [UnInbox](#uninbox)
  - [Chatwoot](#chatwoot)
  - [FreeScout](#freescout)
  - [Zammad](#zammad)
  - [LibreDesk](#libredesk)
  - [Frappe Helpdesk](#frappe-helpdesk)
  - [Messages (La Suite)](#messages-la-suite)
  - [Cerb](#cerb)
- [Comparison at a Glance](#-comparison-at-a-glance)
- [Contributing](#-contributing)

---

## 🟦 SaaS / Hosted Platforms

Commercial, cloud-hosted Unified Email and Communication Inbox platforms. These are not open-source but are included as reference points for feature comparison.

### Front
**Type:** Collaborative shared inbox for teams  
Front is the category-defining shared inbox platform, treating email, chat, and messaging as collaborative conversations rather than private mailboxes. Teams can assign threads, add internal notes, use collision detection to prevent duplicate replies, and route messages by rules . Pricing starts at $25/month on the Starter plan ($300/year), scaling significantly for larger teams . Front's strength is its polished email-native collaboration model, with turnkey connectors for Salesforce and multi-channel telephony .  
**Best for:** Teams wanting a mature, polished shared inbox with deep collaboration features and enterprise integrations, accepting per-seat pricing.

### Missive
**Type:** Collaborative email and chat app  
Missive combines email, chat, and task management in a unified interface. Teams can discuss emails in private threads, assign conversations, and collaborate on replies without forwarding. Positioned as a modern alternative to Front and Hiver for teams wanting email-centric collaboration with built-in chat.

### Hiver
**Type:** Shared Gmail inbox for teams  
Hiver layers shared mailbox functionality directly on top of Gmail, allowing teams to manage support, sales, and operations emails without leaving their existing email client. Features include shared labels, assignments, collision detection, and analytics. Suited for organizations standardized on Gmail wanting team collaboration without a separate application.

### Superhuman
**Type:** Fast email client with team features  
Superhuman is known for its keyboard-driven, blazing-fast email experience, with team features for shared availability and conversation tracking. Focused on individual productivity and speed rather than full shared-inbox collaboration, though it includes some team-oriented capabilities.

### Spark Mail
**Type:** Smart email client with team collaboration  
Spark (Readdle) offers a modern email client with smart inbox prioritization, team collaboration features (shared drafts, comments), and integrations. Available across platforms. Suited for teams wanting a polished email client with collaborative touches rather than a full shared-inbox platform.

### Help Scout
**Type:** Email-first customer support platform  
Help Scout provides shared inboxes for customer support teams with a focus on email-first conversations. Features include assignments, collision detection, saved replies, and a knowledge base. The interface is designed to feel like email rather than a ticketing system, making it accessible for smaller teams.

### Gmelius
**Type:** Collaborative Gmail inbox  
Gmelius extends Gmail with shared inboxes, assignment, collision detection, and workflow automation. Suited for teams already using Gmail who want Hiver-like functionality with a different feature set and pricing model.

### Crisp
**Type:** Omnichannel customer messaging  
Crisp combines live chat, email, and messaging channels into a unified inbox. Focused on customer engagement across website chat, email, and social messaging. Suited for businesses wanting a single inbox for multiple customer communication channels.

---

## 🟩 Open-Source Software

Self-hosted, community-driven Unified Email and Communication Inbox tools. The open-source ecosystem splits between **email-native collaborative inboxes** (UnInbox, Messages) and **help desk platforms with shared mailbox functionality** (Chatwoot, FreeScout, Zammad).

### UnInbox
**Stack:** TypeScript / Nuxt / MySQL / Docker | **License:** AGPL-3.0   
UnInbox is the most direct open-source alternative to Front, Missive, and Hey.com, explicitly designed as a modern email experience for teams and professionals . Features include shared spaces with private comments attached directly to email threads (without exposing internal text to customers), explicit workflow statuses (open, waiting, completed), direct conversation assignment to prevent duplicate replies, unlimited departmental addresses (support, sales, billing) without per-address fees, and new sender screening . Built on a Nuxt/Vue stack with DrizzleORM and MySQL, deployable via Docker . **Important limitation:** Self-hosting requires manual configuration of SMTP ingress, reverse DNS, and IP reputation for reliable delivery; no native mobile apps (responsive web only) .  
**Best for:** Boutique agencies and small operations teams wanting an email-native shared inbox with notes and workflow statuses without per-seat fees, accepting self-hosted email infrastructure complexity.

### Chatwoot
**Stack:** Ruby on Rails / Vue / PostgreSQL / Redis | **License:** MIT (Community Edition)   
Chatwoot is an open-source omnichannel support desk covering email, website live chat, WhatsApp Business, Facebook Messenger, Instagram DMs, SMS, and API-driven custom channels in a single queue . The Community Edition is MIT-licensed and free to self-host, with assignments to individuals and teams, private notes with mentions, typing indicators for collision detection, canned responses, labels, and per-agent workload views . Deployment via Docker Compose or Helm chart. **Trade-off vs Front:** It is support-inbox oriented and weaker than Front for email-first shared drafting, internal collaboration, routing rules, and multi-inbox operations . Enterprise features like SSO/SAML and audit logs require a paid tier, but upgrades are data-preserving .  
**Best for:** Teams needing a single queue for email plus chat and social channels, wanting MIT licensing and Docker-friendly deployment, accepting that email-native collaboration is less polished than Front.

### FreeScout
**Stack:** PHP / MySQL | **License:** AGPL-3.0   
FreeScout is a self-hosted shared mailbox and help desk explicitly positioned as a free Zendesk and Help Scout alternative . Features include shared mailboxes via IMAP/SMTP, assignment, private notes, statuses (active, pending, closed), tags, workflows, and per-user activity views . Deployable on a PHP/MySQL host with a web installer, even on shared hosting. **Trade-offs:** The interface is help-desk shaped rather than email-native, and several advanced modules (tags, workflows, SMS, apps) are separate paid add-ons . Self-hosting requires managing PHP upgrades, TLS renewals, SMTP relay deliverability, and backups .  
**Best for:** Technical teams with a spare VPS or shared hosting wanting a free-forever shared mailbox with help desk features, accepting paid modules for advanced functionality.

### Zammad
**Stack:** Ruby on Rails / PostgreSQL / Elasticsearch | **License:** AGPL-3.0   
Zammad is a mature, web-based open-source help desk and customer support system with 6,017+ GitHub stars and active development . Features include ticketing, ownership, team workflows, SLAs, a knowledge base, email channels, and multi-channel support . Deployment requires Docker Compose or Linux packages with PostgreSQL, Redis, and Elasticsearch/OpenSearch . **Trade-off vs Front:** Zammad treats messages as help-desk tickets rather than preserving Front's lighter, email-native team collaboration model; it is heavier semantically and operationally .  
**Best for:** Organizations needing a serious ticket desk with SLAs and knowledge base, where email is an input channel rather than the primary workplace.

### LibreDesk
**Stack:** Go / PostgreSQL / Docker | **License:** AGPL-3.0   
LibreDesk is a modern open-source email-and-live-chat desk in a compact stack, with 2,682+ GitHub stars as of August 2026 . Features include shared inboxes for email and live chat, assignment, and a modern UI. Deployable via Docker or prebuilt binary with PostgreSQL . **Trade-off:** It is a much younger product with a smaller integration, mobile, reporting, and administration ecosystem than Front .  
**Best for:** Teams wanting a modern, lightweight open-source shared inbox with email and live chat, accepting a younger ecosystem.

### Frappe Helpdesk
**Stack:** Python / Frappe Framework / Vue | **License:** AGPL-3.0   
Frappe Helpdesk provides clean shared support queues with assignments and SLAs, built on the Frappe framework (same ecosystem as ERPNext) . Installation requires a Linux server, domain/DNS, Docker or the easy-install script, and mail account configuration . **Trade-off:** It replaces email-native workflows with a separate ticket queue and a Frappe server to operate .  
**Best for:** Teams already in the Frappe/ERPNext ecosystem wanting helpdesk functionality with SLA support.

### Messages (La Suite)
**Stack:** Python / Django / Postfix / Docker | **License:** Open Source (per project)   
Messages is a collaborative inbox built for La Suite territoriale (French government), with a full communication platform for teams to collaborate on emails through shared or personal mailboxes . Features include smart threading, attachments, MBOX/IMAP import, full-text search with advanced filters, AI summaries/composer/auto-labelling, shared inboxes, shared threads, and OpenID Connect for all accounts . Uses a custom MTA based on Postfix and a Django Rest Framework backend. **Important:** No POP3 or IMAP client support by design; data model is JMAP-inspired . Deploys via Docker Compose.  
**Best for:** Government and public sector teams needing a sovereign, collaborative email inbox with AI features and Keycloak integration.

### Cerb
**Stack:** PHP / MySQL | **License:** Open Source (per project)   
Cerb is a fully customizable, web-based platform for enterprise communication and process automation, used by thousands of teams for 15+ years . It creates high-volume shared inboxes with bot-powered email management, workflow automation via the KATA language, and browser-based coding tools. Integrates with any API-based service. **Trade-off:** Older interface and a steeper learning curve for its automation language; smaller active community (79 stars on the main repository) .  
**Best for:** Organizations needing high-volume shared inboxes with deep, customizable automation, accepting an older UI and learning investment.

---

## 📊 Comparison at a Glance

| Software | License | Stack | Email-Native | Omnichannel | Self-Hosted | Best For |
|----------|---------|-------|--------------|-------------|-------------|----------|
| **Front** | Proprietary | Cloud | ✅ | ✅ | ❌ | Polished email-native collaboration |
| **Missive** | Proprietary | Cloud | ✅ | (Chat) | ❌ | Email + chat collaboration |
| **Hiver** | Proprietary | Gmail | ✅ | ❌ | ❌ | Gmail-based shared inbox |
| **Help Scout** | Proprietary | Cloud | ✅ | Limited | ❌ | Email-first support |
| **Crisp** | Proprietary | Cloud | (Email) | ✅ | ❌ | Omnichannel messaging |
| **UnInbox** | AGPL-3.0 | TypeScript/MySQL | ✅ | ❌ | ✅ | Front alternative (email-native) |
| **Chatwoot** | MIT | Ruby/PostgreSQL | (Support) | ✅ | ✅ | Omnichannel + MIT licensing |
| **FreeScout** | AGPL-3.0 | PHP/MySQL | (Help desk) | ❌ | ✅ | Free-forever shared mailbox |
| **Zammad** | AGPL-3.0 | Ruby/PostgreSQL | (Ticketing) | ✅ | ✅ | Ticket desk with SLAs |
| **LibreDesk** | AGPL-3.0 | Go/PostgreSQL | ✅ (Email+chat) | (Chat) | ✅ | Modern lightweight shared inbox |
| **Frappe Helpdesk** | AGPL-3.0 | Python/Frappe | (Ticket queue) | ❌ | ✅ | Frappe/ERPNext ecosystem |
| **Messages** | Open Source | Python/Django | ✅ | ❌ | ✅ | Sovereign government inbox |
| **Cerb** | Open Source | PHP/MySQL | ✅ (Shared) | (API) | ✅ | High-volume + automation |

---

## 🤝 Contributing

Contributions are welcome! If you know of an open-source Unified Email or Communication Inbox tool that should be listed here, please open a pull request with:

- Project name and URL
- Brief description (1–2 sentences)
- Stack and license
- Why it stands out

Please ensure the project is actively maintained (releases within the last 12 months) and genuinely open-source. Note that the open-source ecosystem **splits** between email-native collaborative inboxes (UnInbox, Messages) that most closely replicate Front/Missive, and help desk platforms (Chatwoot, FreeScout, Zammad) that add shared mailbox functionality but treat email as a support channel rather than a collaborative workspace. UnInbox is currently the closest open-source equivalent to Front's email-native team collaboration model.

---

## 📄 License

This list is released under CC0 1.0 Universal (Public Domain). The software projects listed retain their respective licenses.

---

⭐ **If this list helped you discover a useful tool, please star the repo!** ⭐
