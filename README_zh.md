# FlowPilot 3.0 - 智能化、可视化的流程自动化系统
致力于提供企业级的统一工作流解决方案

[![Python](https://img.shields.io/badge/Python-3.12-3776AB?logo=python&logoColor=white)](https://www.python.org/)
[![Django](https://img.shields.io/badge/Django-5.2-092E20?logo=django&logoColor=white)](https://www.djangoproject.com/)
[![React](https://img.shields.io/badge/React-18.x-61DAFB?logo=react&logoColor=black)](https://reactjs.org/)
[![MUI](https://img.shields.io/badge/MUI-5.x-007FFF?logo=mui&logoColor=white)](https://mui.com/)
[![License](https://img.shields.io/badge/license-AGPL%20v3-blue)](https://www.gnu.org/licenses/agpl-3.0)

[English](./README.md) | 简体中文

## 🚀 全新出发的 FlowPilot 3.0

FlowPilot 是一个基于 Django 开发的开源流程自动化平台。历经多个版本的迭代与重构，FlowPilot 3.0 在可视化、灵活性和扩展性上实现了质的飞跃。

3.0 版本的核心是「让复杂的业务流程变得简单可视，让个性化的定制需求触手可及」。不仅重铸了流程与表单设计器，更构建了一套强大的扩展框架，旨在成为企业数字化转型中最核心的流程引擎。

## 功能演示
[![功能演示](https://img.youtube.com/vi/IpLePpajyfU/0.jpg)](https://www.youtube.com/watch?v=IpLePpajyfU)

## ✨ 核心特性

### 🎯 革命性的可视化设计
- **拖拽式流程设计器**：无需繁杂的配置，通过直观的拖拽连线即可完成复杂业务流程的建模。支持条件分支、并行任务、hook等高级节点。
- **智能表单设计器**：强大的可视化表单构建工具，提供丰富的字段类型（文本、数字、下拉框、人员选择、附件等），布局随心所欲。
- **实时预览与验证**：设计流程时实时预览效果，内置流程逻辑校验，提前规避设计错误。
- **流程配置支持多版本**：可以配置多个版本的流程，并轻松测试和切换版本。

### 🔧 极致的灵活性与扩展性
- **插件化架构**：为几乎所有关键节点都提供了插件扩展能力（如自定义动作、权限验证、通知方式等）。您的独特业务逻辑可以像搭积木一样轻松接入。
- **强大的 API 体系**：提供全面、清晰的 RESTful API，便于与客服系统、CMDB、监控系统、CI/CD、OA 等第三方系统无缝集成。
- **高度可定制的权限模型**：支持基于角色、部门、甚至特定业务条件的精细权限控制。

### 💼 开箱即用的企业级功能
- **多类型工单支持**：轻松管理 IT 运维、人事审批、财务报销、客户服务等各类流程。
- **自动化与智能路由**：支持基于表单数据的条件路由，自动指派处理人，实现工单的智能化流转。
- **详尽的审计日志**：完整记录工单从创建到关闭的每一个操作，满足合规与审计要求。
- **多租户支持（可选）**：为 SaaS 服务商或大型集团企业提供数据隔离能力。

## 🛠️ 安装与部署

1. 下载docker-compose相关文件
```bash
wget https://raw.githubusercontent.com/abubakarkhalid637/flowpilot/refs/heads/master/docker_compose_deploy/docker-compose.yml
wget https://raw.githubusercontent.com/abubakarkhalid637/flowpilot/refs/heads/master/docker_compose_deploy/.env
```
2. 修改 `.env` 文件（请至少修改密码部分）
3. 启动docker-compose
```bash
docker-compose up -d
```
4. 创建admin用户
```bash
cd /app/flowpilot
python manage.py createsuperuser
```
5. 使用创建的邮箱和密码登录 FlowPilot

## 📖 深入探索

- 📚 **完整文档**: https://flowpilot.readthedocs.io
- 🔌 **Hook开发指南** - 学习如何为 FlowPilot 开发自定义插件。
- 🌐 **API 参考**: https://documenter.getpostman.com/view/15031929/2sB3WyJbap

## 🗺️ 项目规划
[项目规划](./Roadmap_zh.md)

## ❓ 获取帮助

- 📝 **GitHub Issues** - 提交 Bug 报告和功能请求。
- 📧 **联系方式**: abubakarkhalid637@gmail.com

如果 FlowPilot 对您有帮助，请给一个 ⭐️ Star 支持！

## 许可证

本项目基于 [AGPLv3](https://www.gnu.org/licenses/agpl-3.0) 协议开源。
