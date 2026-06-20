<div align="center">

# 🎮 Xbox Admin

**企业信息化系统智能搭建工具**

[![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)](https://spring.io/projects/spring-boot)
[![Vue.js](https://img.shields.io/badge/Vue.js-4FC08D?style=flat-square&logo=vuedotjs&logoColor=white)](https://vuejs.org/)
[![Flowable](https://img.shields.io/badge/Flowable-7.1-1B8FE0?style=flat-square&logo=flowable&logoColor=white)](https://www.flowable.com/)
[![MyBatis-Plus](https://img.shields.io/badge/MyBatis--Plus-3.5-red?style=flat-square)](https://baomidou.com/)
[![License](https://img.shields.io/badge/License-MIT-yellow?style=flat-square)](LICENSE)

[English](./README_EN.md) | 简体中文

</div>

---

## 📖 项目介绍

**Xbox Admin** 是一个企业信息化系统智能搭建工具，采用前后端分离架构，集成了 **RBAC 权限管理**、**AI 智能对话**、**BPM 流程引擎**、**低代码模型**、**文档解析**、**调度任务** 六大核心能力。所有后端管理能力通过 MCP 工具协议暴露给大语言模型，用户可用自然语言完成所有管理操作。

系统还提供**业务字典治理**（业务分类 / 业务目录 / 业务模型 / 业务元素 / 数据元素 + 本体血缘 + 业务探索）和**主从库读写分离**能力，支持企业级数据治理与高性能数据访问。

### ✨ 核心特性

<details open>
<summary><b>🤖 AI 智能能力</b></summary>

| 特性 | 说明 |
|------|------|
| **AI 原生架构** | 所有后端能力通过 MCP 工具暴露给 LLM，六 Agent（Admin / Flow / Model / Office / Schedule / Reverse）智能协作 |
| **多模态 AI 对话** | 图片理解 + 文件解析 + 工具调用 + 流式打字机效果，兼容任意 OpenAI API |
| **专家模式聊天室** | 多 Agent 顺序协作讨论，自动生成总结 |
| **RAG 知识库** | 文档摄入、自动分块、向量检索增强生成，支持 Simple / OpenAI Embedding |

</details>

<details open>
<summary><b>🔐 权限与安全</b></summary>

| 特性 | 说明 |
|------|------|
| **完整 RBAC 权限** | 用户 / 角色 / 部门 / 员工 / 分组 / 菜单 / 按钮 / 数据级权限，声明式注解校验 |
| **多租户隔离** | 完整的租户数据隔离，租户上下文自动传播 |
| **前后端加密** | HMAC 签名 + AES 加密 + 防重放 + 防篡改 + XSS / SQL 注入检测 |
| **国际化** | 完整的中文 / 英文双语支持 |

</details>

<details open>
<summary><b>🛠️ 低代码与数据治理</b></summary>

| 特性 | 说明 |
|------|------|
| **低代码引擎** | 动态建表、动态 CRUD、主子关系、版本管理、数据库逆向、业务字典、字段级密级加密 |
| **业务字典治理** | 业务分类 / 业务目录 / 业务模型 / 业务元素 / 数据元素五级体系，业务-数据双轨溯源 |
| **本体血缘** | 从业务概念到物理实现的完整血缘图谱，6 种节点 + 5 种关系边 |
| **业务探索** | 图谱可视化 + 查询方案（自动构建多表 JOIN SQL） |
| **主从库读写分离** | 服务层动态路由，轮询负载均衡，从库缓存双模式（内存 / Redis），自动故障转移 |

</details>

<details open>
<summary><b>⚙️ 流程与调度</b></summary>

| 特性 | 说明 |
|------|------|
| **BPMN 流程设计** | 基于 Flowable 7.1 + bpmn-js 的可视化流程设计，与低代码模型深度集成 |
| **文档解析** | 支持 txt / md / json / csv 多格式文档解析 |
| **调度任务** | 支持 Spring Scheduler / XXL-JOB 双框架，cron / fixed_rate / fixed_delay 多调度类型 |

</details>

<details open>
<summary><b>🚀 工程化能力</b></summary>

| 特性 | 说明 |
|------|------|
| **快速搭建** | 开箱即用，无需复杂配置即可启动 |
| **轻量部署** | H2 嵌入式数据库，单 JAR 部署，支持 GraalVM Native Image / MySQL / Redis |

</details>

---

## 🏗️ 软件架构

| 层级 | 技术栈 | 说明 |
|:----:|:------:|------|
| **后端** | `Spring Boot` | 企业级 Java 应用框架 |
| **前端** | `Vue.js` | 渐进式 JavaScript 框架 |
| **工作流** | `Flowable 7.1` | 业务流程引擎 |
| **持久层** | `MyBatis-Plus` | MyBatis 增强工具 |
| **数据库** | `MySQL` / `H2` | 关系型数据库 |
| **缓存** | `Redis` | 分布式缓存 |

---

## 📁 项目结构

```
xbox-admin/
├── xbox-admin.zip.*      # 程序文件（分片压缩，共 12 个包）
├── application.yml      # 配置文件
├── logback-spring.xml   # 日志配置
├── chat.md               # 聊天示例
├── chat.png              # 系统截图
├── LICENSE               # 开源协议
└── README.md             # 项目说明
```

---

## 🚀 快速开始

### 1️⃣ 解压安装包

> 受程序包大小提交限制，已分片压缩为 **12 个 ZIP 包**，需全部下载后解压。

### 2️⃣ 启动主服务

运行 `xbox-admin.exe` 启动后端服务。

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

<sub>© 2025 Xbox Admin. All rights reserved.</sub>

</div>
