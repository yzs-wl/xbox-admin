<div align="center">

# 🎮 Xbox Admin

**企业信息化系统智能搭建工具**

[![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)](https://spring.io/projects/spring-boot)
[![Vue.js](https://img.shields.io/badge/Vue.js-4FC08D?style=flat-square&logo=vuedotjs&logoColor=white)](https://vuejs.org/)
[![License](https://img.shields.io/badge/License-MIT-yellow?style=flat-square)](LICENSE)

[English](./README_EN.md) | 简体中文

</div>

---

## 📖 项目介绍

**Xbox Admin** 是一款企业信息化系统智能搭建工具，基于 **Spring Boot + Vue.js** 技术栈构建。旨在帮助企业快速搭建和管理信息化系统，提供从应用管理、服务治理到数据模型管控的全流程能力。

### 核心特性

- 🚀 **快速搭建** — 开箱即用，无需复杂配置即可启动
- 🤖 **AI 驱动** — 支持大模型智能对话，通过自然语言驱动系统各模块
- 📦 **全生命周期管理** — 涵盖应用注册、审核、上下线、分类管理等完整流程
- 🔒 **安全可控** — 统一认证授权，操作审计日志全覆盖

---

## 🏗️ 软件架构

| 层级 | 技术栈 | 说明 |
|------|--------|------|
| **后端** | Spring Boot | 企业级 Java 应用框架 |
| **前端** | Vue.js | 渐进式 JavaScript 框架 |
| **工作流** | Flowable | 业务流程引擎 |
| **持久层** | MyBatis-Plus | MyBatis 增强工具 |
| **数据库** | MySQL / H2 | 关系型数据库 |

---

## 📁 项目结构

```
xbox-admin/
├── boot/          # 后端工程（Spring Boot 多模块）
├── web/           # 前端工程（Vue.js + Vite）
├── data/          # 数据库文件
├── base.md        # 需求文档
├── platform.md    # 详细设计文档
└── README.md      # 项目说明
```

---

## 🚀 快速开始

### 1. 解压安装包

> 受程序包大小提交限制，已分片压缩为 **12 个 ZIP 包**，需全部解压。

### 2. 启动主服务

运行 `xbox-admin.exe` 启动后端服务。

### 3. 访问系统

| 项目 | 说明 |
|------|------|
| 访问地址 | [http://127.0.0.1:8080](http://127.0.0.1:8080) |
| 默认用户名 | `admin` |
| 默认密码 | `admin123` |

---

## 🤖 AI 智能对话配置

登录系统后，进入 **智能对话 → 模型配置** 菜单，选择对应模型并设置 API Key 即可使用大模型对话方式驱动系统各个模块。

> 当然，也可以不使用大模型，手工操作各模块菜单完成数据录入。

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
