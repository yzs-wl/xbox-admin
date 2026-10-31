<div align="center">

# 🎮 Xbox Admin

**企业信息化系统智能搭建工具**

[![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)](https://spring.io/projects/spring-boot)
[![Vue.js](https://img.shields.io/badge/Vue.js-4FC08D?style=flat-square&logo=vuedotjs&logoColor=white)](https://vuejs.org/)
[![Spring AI](https://img.shields.io/badge/Spring%20AI-1.1-6DB33F?style=flat-square&logo=spring&logoColor=white)](https://spring.io/projects/spring-ai)
[![Flowable](https://img.shields.io/badge/Flowable-7.1-1B8FE0?style=flat-square&logo=flowable&logoColor=white)](https://www.flowable.com/)
[![License](https://img.shields.io/badge/License-Apache%202.0-blue?style=flat-square)](LICENSE)

[English](./README_EN.md) | 简体中文

</div>

---

## 📖 项目介绍

**Xbox Admin** 是一个企业信息化系统智能搭建工具，采用前后端分离架构，集成了 **RBAC 权限管理**、**AI 智能对话**、**设计中心**、**BPM 流程引擎**、**低代码模型**、**文档解析**、**调度任务** 七大核心能力。所有后端管理能力通过 MCP 工具协议暴露给大语言模型，用户可用自然语言完成所有管理操作。

系统还提供**业务字典治理**（业务分类 / 业务目录 / 业务模型 / 业务元素 / 数据元素 + 本体血缘 + 业务探索）和**主从库读写分离**能力，支持企业级数据治理与高性能数据访问。

系统内置**设计中心**，提供 EA 五视图建模、逻辑数据模型、详细设计图与设计资产沉淀，并通过落地映射 / 模型转换 / 一键拉通 / 漂移检测 / 基线管控实现**设计态与运行态双向打通**，支持从需求到运行的全链路追溯。

### ✨ 核心特性

<details open>
<summary><b>🤖 AI 智能能力</b></summary>

| 特性 | 说明 |
|------|------|
| **AI 原生架构** | 所有后端能力通过 MCP 工具暴露给 LLM，七 Agent（Admin / Flow / Model / Reverse / Office / Schedule / Skill）智能协作 |
| **多模态 AI 对话** | 图片理解 + 文件解析 + 工具调用 + 流式打字机效果，兼容任意 OpenAI API |
| **专家模式聊天室** | 多 Agent 多轮顺序协作讨论，自动生成总结 |
| **RAG 知识库** | 文档摄入、自动分块、向量检索增强生成，支持 Simple / OpenAI Embedding |
| **AI 技能系统** | 服务 / 模型 / 流程统一抽象为可发现、可调用的技能，支持 Markdown 描述与反向生成 |
| **Playbook 经验固化** | 成功调用套路语义化保存到向量知识库，下次自动检索复用 |

</details>

<details open>
<summary><b>🔐 权限与安全</b></summary>

| 特性 | 说明 |
|------|------|
| **完整 RBAC 权限** | 用户 / 角色 / 部门 / 员工 / 分组 / 菜单 / 按钮 / 数据级权限，声明式注解校验 |
| **多租户隔离** | 完整的租户数据隔离，租户上下文自动传播 |
| **SSO 单点登录** | 支持 Keycloak / GitHub / WeChat / 企业微信 / Azure AD / Okta / Google / 钉钉 / 飞书 九大 Provider |
| **前后端加密** | HMAC 签名 + AES 加密 + 防重放 + 防篡改 + XSS / SQL 注入检测，7 层可配置开关 |
| **登录安全** | 失败锁定 + 验证码 + 密码复杂度 / 历史 / 过期策略 |
| **企业级能力** | 幂等性防重、通知中心（站内 / 邮件 / Webhook）、多时区、AI 成本管控与配额 |
| **国际化** | 完整的中文 / 英文双语支持 |

</details>

<details open>
<summary><b>🛠️ 低代码与数据治理</b></summary>

| 特性 | 说明 |
|------|------|
| **低代码引擎** | 动态建表、动态 CRUD、主子关系、版本管理、数据库逆向、业务字典、字段级密级加密、视图设计器、服务设计、业务规则 |
| **业务字典治理** | 业务分类 / 业务目录 / 业务模型 / 业务元素 / 数据元素五级体系，业务-数据双轨溯源 |
| **本体血缘** | 从业务概念到物理实现的完整血缘图谱，6 种节点 + 5 种关系边 |
| **业务探索** | 图谱可视化 + 查询方案（自动构建多表 JOIN SQL） |
| **主从库读写分离** | 服务层动态路由，轮询负载均衡，从库缓存双模式（内存 / Redis），自动故障转移 |

</details>

<details open>
<summary><b>🎨 设计中心</b></summary>

| 特性 | 说明 |
|------|------|
| **EA 企业架构** | 业务域 / 业务能力 / 应用 / 技术 / 安全五视图对象与分层管理，能力地图 + 架构对齐校验 |
| **统一设计对象** | 领域 / 项目树 + 设计对象统一版本管理，9 种对象关系（包含 / 实现 / 映射 / 依赖等）、批注评审、需求追溯与变更影响分析 |
| **逻辑数据建模** | 逻辑模型 / 属性 / ER 图 / 字段级血缘（FK / 数据元素 / 物理列三向溯源），一键导出 8 种方言 DDL（MySQL / PostgreSQL / Oracle / 达梦 / 人大金仓等） |
| **设计态-运行态打通** | 设计对象 ↔ 运行实体落地映射（已关联 / 已落地 / 偏离）；逻辑模型 ↔ 物理模型双向转换；流程图一键落地 Flowable；业务规则 / 接口细化一键生成运行态规则与服务 |
| **一键拉通与漂移检测** | 五视图设计对象一键落地为详细设计成果物（领域 / 微服务 / 逻辑模型 / 集成定义）；物理模型与运行表列自动比对，生成增量 ALTER 脚本并回写落地状态 |
| **基线与变更管控** | 设计基线快照 / 版本漂移对比 / 基线恢复 / 对象回滚，字段级版本差异；变更单接入 Flowable 多环节审批，评审通过自动固化基线 |
| **AI 设计** | AI 生成逻辑模型 / 接口定义（自动落入设计模型）、架构遵从 / 命名规范 / 模型一致性智能审查 |
| **详细设计图** | 类图 / 用例图 / 组件图 / 部署图 / 状态图 / 活动图 / 时序图 / 流程图 8 类图，自动布局落库 |
| **治理与拓扑** | 数据资产地图、数据流转全链路血缘、集成关系图谱、部署拓扑、安全架构拓扑 |
| **资产与度量** | 设计资产库跨项目复用、设计模板 / 设计规范、UI 主题、技术路线、提示词模板、合规自动检查与设计度量审计 |

</details>

<details open>
<summary><b>⚙️ 流程与调度</b></summary>

| 特性 | 说明 |
|------|------|
| **BPMN 流程设计** | 基于 Flowable 7.1 + bpmn-js 的可视化流程设计，与低代码模型深度集成 |
| **文档解析** | 支持 txt / md / json / csv / docx / xlsx / pptx / pdf / mpp / vsdx 多格式文档解析 |
| **调度任务** | 支持 Spring Scheduler / XXL-JOB 双框架，cron / fixed_rate / fixed_delay / one_shot 多调度类型 |

</details>

<details open>
<summary><b>🚀 工程化能力</b></summary>

| 特性 | 说明 |
|------|------|
| **快速搭建** | 开箱即用，无需复杂配置即可启动 |
| **轻量部署** | H2 嵌入式数据库，单 JAR 部署，支持 GraalVM Native Image / MySQL / PostgreSQL / Redis |

</details>

---

## 🏗️ 软件架构

| 层级 | 技术栈 | 说明 |
|:----:|:------:|------|
| **后端** | `Spring Boot 3` + `Java 21` | 企业级 Java 应用框架 |
| **AI** | `Spring AI` + `MCP` | LLM 集成与工具协议 |
| **前端** | `Vue 3` + `Element Plus` | 渐进式 JavaScript 框架 |
| **工作流** | `Flowable 7.1` | 业务流程引擎 |
| **持久层** | `Spring Data JPA` | ORM / 数据访问 |
| **数据库** | `H2` / `MySQL` / `PostgreSQL` | 关系型数据库 |
| **缓存** | `Redis`（可选） | 分布式缓存 / 会话存储 |

---

## 📁 项目结构

```
xbox-admin/
├── xbox-admin.zip.001~003   # Windows 版程序（分片压缩，共 3 个包）
├── linux/                   # Linux 版程序（分片压缩 + 配置文件）
├── application.yaml         # 配置文件
├── LICENSE                  # 开源协议（Apache 2.0）
├── README.md                # 项目说明（中文）
└── README_EN.md             # 项目说明（英文）
```

---

## 🚀 快速开始

### 1️⃣ 解压安装包

> 受程序包大小提交限制，已分片压缩为 **3 个 ZIP 包**（`linux/` 目录下为 Linux 版），需全部下载后解压至同一目录。

### 2️⃣ 启动服务

- **Windows**：运行 `xbox-admin.exe` 启动服务
- **Linux**：解压 `linux/` 下的分片包，运行 `xbox-admin`

### 3️⃣ 访问系统

| 项目 | 说明 |
|------|------|
| 访问地址 | [http://127.0.0.1:8080](http://127.0.0.1:8080) |
| 默认用户名 | `admin` |
| 默认密码 | `admin123` |

---

## 🤖 AI 智能对话配置

登录系统后，进入 **智能对话 → 模型配置** 菜单，选择对应模型并设置 API Key 即可使用大模型对话方式驱动系统各个模块。

> 💡 也可以不使用大模型，手工操作各模块菜单完成数据录入。

### 推荐模型 — DeepSeek

性价比高，可在 [DeepSeek API Keys](https://platform.deepseek.com/api_keys) 页面注册申请 API Key。

---

## 📧 技术支持

如有任何问题或建议，欢迎联系：

- 邮箱：[xbox_admin@163.com](mailto:xbox_admin@163.com)

---

<div align="center">

<sub>© 2025-2026 Xbox Admin. All rights reserved.</sub>

</div>
