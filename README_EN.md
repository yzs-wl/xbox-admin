<div align="center">

# 🎮 Xbox Admin

**Enterprise Information System Intelligent Builder**

[![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)](https://spring.io/projects/spring-boot)
[![Vue.js](https://img.shields.io/badge/Vue.js-4FC08D?style=flat-square&logo=vuedotjs&logoColor=white)](https://vuejs.org/)
[![Spring AI](https://img.shields.io/badge/Spring%20AI-1.1-6DB33F?style=flat-square&logo=spring&logoColor=white)](https://spring.io/projects/spring-ai)
[![Flowable](https://img.shields.io/badge/Flowable-7.1-1B8FE0?style=flat-square&logo=flowable&logoColor=white)](https://www.flowable.com/)
[![License](https://img.shields.io/badge/License-Apache%202.0-blue?style=flat-square)](LICENSE)

English | [简体中文](./README.md)

</div>

---

## 📖 Introduction

**Xbox Admin** is an enterprise information system intelligent builder based on **Spring Boot + Vue.js**. It adopts a front-end/back-end separation architecture and integrates six core capabilities: **RBAC Permission Management**, **AI Intelligent Dialogue**, **BPM Workflow Engine**, **Low-Code Model**, **Document Parsing**, and **Scheduled Tasks**. All backend management capabilities are exposed to large language models via the MCP tool protocol, allowing users to perform all administrative operations through natural language.

The system also provides **Business Dictionary Governance** (Business Category / Business Catalog / Business Model / Business Element / Data Element + Ontology Lineage + Business Exploration) and **Master-Slave Read/Write Separation** capabilities, supporting enterprise-grade data governance and high-performance data access.

### ✨ Key Features

<details open>
<summary><b>🤖 AI Capabilities</b></summary>

| Feature | Description |
|---------|-------------|
| **AI-Native Architecture** | All backend capabilities exposed to LLM via MCP tools; seven Agents (Admin / Flow / Model / Reverse / Office / Schedule / Skill) collaborate intelligently |
| **Multimodal AI Dialogue** | Image understanding + file parsing + tool calling + streaming typewriter effect; compatible with any OpenAI API |
| **Expert Mode Chat Room** | Multi-agent multi-round collaborative discussion with auto-generated summaries |
| **RAG Knowledge Base** | Document ingestion, auto-chunking, vector retrieval-augmented generation; supports Simple / OpenAI Embedding |
| **AI Skill System** | Services / models / workflows abstracted as discoverable, invocable skills with Markdown descriptions and reverse generation |
| **Playbook Experience Solidification** | Successful invocation patterns saved semantically to a vector knowledge base for automatic retrieval and reuse |

</details>

<details open>
<summary><b>🔐 Permission & Security</b></summary>

| Feature | Description |
|---------|-------------|
| **Full RBAC Permissions** | User / Role / Department / Employee / Group / Menu / Button / Data-level permissions with declarative annotation validation |
| **Multi-Tenant Isolation** | Complete tenant data isolation with automatic tenant context propagation |
| **SSO Single Sign-On** | Supports nine providers: Keycloak / GitHub / WeChat / WeCom / Azure AD / Okta / Google / DingTalk / Feishu |
| **Frontend-Backend Encryption** | HMAC signature + AES encryption + anti-replay + anti-tamper + XSS / SQL injection detection, with 7 configurable layers |
| **Login Security** | Failure lockout + captcha + password complexity / history / expiration policies |
| **Enterprise Capabilities** | Idempotency protection, Notification Center (In-app / Email / Webhook), multi-timezone, AI cost control & quotas |
| **Internationalization** | Full Chinese / English bilingual support |

</details>

<details open>
<summary><b>🛠️ Low-Code & Data Governance</b></summary>

| Feature | Description |
|---------|-------------|
| **Low-Code Engine** | Dynamic table creation, dynamic CRUD, master-child relationships, version management, database reverse engineering, business dictionary, field-level classification encryption, view designer, service designer, business rules |
| **Business Dictionary Governance** | Five-tier system: Business Category / Business Catalog / Business Model / Business Element / Data Element with business-data dual-track traceability |
| **Ontology Lineage** | Complete lineage graph from business concept to physical implementation, 6 node types + 5 relationship types |
| **Business Exploration** | Graph visualization + query schemes (auto-generated multi-table JOIN SQL) |
| **Master-Slave Read/Write Separation** | Service-layer dynamic routing, round-robin load balancing, dual slave cache modes (Memory / Redis), automatic failover |

</details>

<details open>
<summary><b>⚙️ Workflow & Scheduling</b></summary>

| Feature | Description |
|---------|-------------|
| **BPMN Workflow Design** | Visual workflow design based on Flowable 7.1 + bpmn-js, deeply integrated with low-code models |
| **Document Parsing** | Supports txt / md / json / csv / docx / xlsx / pptx / pdf / mpp / vsdx multi-format document parsing |
| **Scheduled Tasks** | Supports Spring Scheduler / XXL-JOB dual frameworks with cron / fixed_rate / fixed_delay / one_shot scheduling types |

</details>

<details open>
<summary><b>🚀 Engineering Capabilities</b></summary>

| Feature | Description |
|---------|-------------|
| **Quick Setup** | Ready to use out of the box, no complex configuration required |
| **Lightweight Deployment** | H2 embedded database, single JAR deployment; supports GraalVM Native Image / MySQL / PostgreSQL / Redis |

</details>

---

## 🏗️ Software Architecture

| Layer | Technology | Description |
|:-----:|:----------:|-------------|
| **Backend** | `Spring Boot 3` + `Java 21` | Enterprise-grade Java application framework |
| **AI** | `Spring AI` + `MCP` | LLM integration and tool protocol |
| **Frontend** | `Vue 3` + `Element Plus` | Progressive JavaScript framework |
| **Workflow** | `Flowable 7.1` | Business process engine |
| **Persistence** | `Spring Data JPA` | ORM / data access |
| **Database** | `H2` / `MySQL` / `PostgreSQL` | Relational database |
| **Cache** | `Redis` (optional) | Distributed cache / session storage |

---

## 📁 Project Structure

```
xbox-admin/
├── xbox-admin.zip.001~003   # Windows program (split-compressed, 3 archives)
├── linux/                   # Linux program (split archives + config file)
├── application.yaml         # Configuration file
├── LICENSE                  # Open source license (Apache 2.0)
├── README.md                # Project documentation (Chinese)
└── README_EN.md             # Project documentation (English)
```

---

## 🚀 Quick Start

### 1️⃣ Extract the Installation Package

> Due to package size restrictions, the program has been split-compressed into **3 ZIP archives** (the `linux/` directory contains the Linux version). Download all archives and extract them into the same directory.

### 2️⃣ Launch the Service

- **Windows**: Run `xbox-admin.exe` to start the service
- **Linux**: Extract the split archives under `linux/`, then run `java -jar xbox-admin.jar` (JDK 21+ required)

### 3️⃣ Access the System

| Item | Description |
|------|-------------|
| URL | [http://127.0.0.1:8080](http://127.0.0.1:8080) |
| Default Username | `admin` |
| Default Password | `admin123` |

---

## 🤖 AI Dialogue Configuration

After logging in, navigate to **Intelligent Dialogue → Model Configuration** in the menu, select the desired model and set the API Key to start driving system modules via LLM-powered conversations.

> 💡 You can also skip the LLM and manually operate each module to complete data entry.

### Recommended Model — DeepSeek

Offers excellent value for money. You can register and obtain an API Key at [DeepSeek API Keys](https://platform.deepseek.com/api_keys).

---

## 📧 Support

If you have any questions or suggestions, feel free to contact us:

- Email: [xbox_admin@163.com](mailto:xbox_admin@163.com)

---

<div align="center">

<sub>© 2025-2026 Xbox Admin. All rights reserved.</sub>

</div>
