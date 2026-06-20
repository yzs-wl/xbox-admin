<div align="center">

# 🎮 Xbox Admin

**Enterprise Information System Intelligent Builder**

[![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)](https://spring.io/projects/spring-boot)
[![Vue.js](https://img.shields.io/badge/Vue.js-4FC08D?style=flat-square&logo=vuedotjs&logoColor=white)](https://vuejs.org/)
[![Flowable](https://img.shields.io/badge/Flowable-7.1-1B8FE0?style=flat-square&logo=flowable&logoColor=white)](https://www.flowable.com/)
[![MyBatis-Plus](https://img.shields.io/badge/MyBatis--Plus-3.5-red?style=flat-square)](https://baomidou.com/)
[![License](https://img.shields.io/badge/License-MIT-yellow?style=flat-square)](LICENSE)

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
| **AI-Native Architecture** | All backend capabilities exposed to LLM via MCP tools; six Agents (Admin / Flow / Model / Office / Schedule / Reverse) collaborate intelligently |
| **Multimodal AI Dialogue** | Image understanding + file parsing + tool calling + streaming typewriter effect; compatible with any OpenAI API |
| **Expert Mode Chat Room** | Multi-agent sequential collaborative discussion with auto-generated summaries |
| **RAG Knowledge Base** | Document ingestion, auto-chunking, vector retrieval-augmented generation; supports Simple / OpenAI Embedding |

</details>

<details open>
<summary><b>🔐 Permission & Security</b></summary>

| Feature | Description |
|---------|-------------|
| **Full RBAC Permissions** | User / Role / Department / Employee / Group / Menu / Button / Data-level permissions with declarative annotation validation |
| **Multi-Tenant Isolation** | Complete tenant data isolation with automatic tenant context propagation |
| **Frontend-Backend Encryption** | HMAC signature + AES encryption + anti-replay + anti-tamper + XSS / SQL injection detection |
| **Internationalization** | Full Chinese / English bilingual support |

</details>

<details open>
<summary><b>🛠️ Low-Code & Data Governance</b></summary>

| Feature | Description |
|---------|-------------|
| **Low-Code Engine** | Dynamic table creation, dynamic CRUD, master-child relationships, version management, database reverse engineering, business dictionary, field-level encryption |
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
| **Document Parsing** | Supports txt / md / json / csv multi-format document parsing |
| **Scheduled Tasks** | Supports Spring Scheduler / XXL-JOB dual frameworks with cron / fixed_rate / fixed_delay scheduling types |

</details>

<details open>
<summary><b>🚀 Engineering Capabilities</b></summary>

| Feature | Description |
|---------|-------------|
| **Quick Setup** | Ready to use out of the box, no complex configuration required |
| **Lightweight Deployment** | H2 embedded database, single JAR deployment; supports GraalVM Native Image / MySQL / Redis |

</details>

---

## 🏗️ Software Architecture

| Layer | Technology | Description |
|:-----:|:----------:|-------------|
| **Backend** | `Spring Boot` | Enterprise-grade Java application framework |
| **Frontend** | `Vue.js` | Progressive JavaScript framework |
| **Workflow** | `Flowable 7.1` | Business process engine |
| **Persistence** | `MyBatis-Plus` | Enhanced MyBatis toolkit |
| **Database** | `MySQL` / `H2` | Relational database |
| **Cache** | `Redis` | Distributed cache |

---

## 📁 Project Structure

```
xbox-admin/
├── xbox-admin.zip.*      # Program files (split-compressed, 12 archives)
├── application.yml      # Configuration file
├── logback-spring.xml   # Logging configuration
├── chat.md               # Chat example
├── chat.png              # System screenshot
├── LICENSE               # Open source license
└── README.md             # Project documentation
```

---

## 🚀 Quick Start

### 1️⃣ Extract Installation Package

> Due to package size restrictions, the project has been split-compressed into **12 ZIP archives**. All must be downloaded and extracted.

### 2️⃣ Launch the Service

Run `xbox-admin.exe` to start the backend service.

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

<sub>© 2025 Xbox Admin. All rights reserved.</sub>

</div>
