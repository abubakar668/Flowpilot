# FlowPilot 3.0 - Intelligent and Visual Process Automation System
Dedicated to providing enterprise-grade unified workflow solutions

[![Python](https://img.shields.io/badge/Python-3.12-3776AB?logo=python&logoColor=white)](https://www.python.org/)
[![Django](https://img.shields.io/badge/Django-5.2-092E20?logo=django&logoColor=white)](https://www.djangoproject.com/)
[![React](https://img.shields.io/badge/React-18.x-61DAFB?logo=react&logoColor=black)](https://reactjs.org/)
[![MUI](https://img.shields.io/badge/MUI-5.x-007FFF?logo=mui&logoColor=white)](https://mui.com/)
[![License](https://img.shields.io/badge/license-AGPL%20v3-blue)](https://www.gnu.org/licenses/agpl-3.0)

[English](./README.md) | [简体中文](./README_zh.md)

## 🚀 FlowPilot 3.0 - A Fresh Start

FlowPilot is an open-source process automation platform built with Django. After multiple iterations and refactoring cycles, FlowPilot 3.0 achieves a qualitative leap in visualization, flexibility, and scalability.

The core of version 3.0 is "making complex business processes simple and visual, making personalized customization needs within reach." With rebuilt process and form designers, plus a powerful extension framework, FlowPilot aims to become the most core process engine in enterprise digital transformation.

## Feature Demo
[![Feature Demo](https://img.youtube.com/vi/IpLePpajyfU/0.jpg)](https://www.youtube.com/watch?v=IpLePpajyfU)

## ✨ Core Features

### 🎯 Revolutionary Visual Design
- **Drag-and-Drop Process Designer**: Complete complex business process modeling through intuitive drag-and-drop connections. Supports conditional branches, parallel tasks, hooks, and more.
- **Smart Form Designer**: Powerful visual form building tool with rich field types (text, numbers, dropdowns, personnel selection, attachments, etc.) and flexible layouts.
- **Real-time Preview & Validation**: Real-time preview during process design with built-in process logic validation to prevent design errors early.
- **Multi-Version Process Configuration**: Configure multiple versions of processes and easily test and switch between versions.

### 🔧 Ultimate Flexibility & Extensibility
- **Plugin Architecture**: Plugin extension capabilities for almost all key nodes (custom actions, permission validation, notification methods, etc.). Your unique business logic integrates like building blocks.
- **Powerful API System**: Comprehensive RESTful APIs for seamless integration with customer service systems, CMDB, monitoring systems, CI/CD, OA, and other third-party systems.
- **Highly Customizable Permission Model**: Fine-grained permission control based on roles, departments, or specific business conditions.

### 💼 Enterprise-Ready Features Out of the Box
- **Multi-Type Ticket Support**: Manage IT operations, HR approvals, financial reimbursements, customer service, and more.
- **Automation & Smart Routing**: Conditional routing based on form data, automatic assignee assignment, and intelligent ticket flow.
- **Comprehensive Audit Logs**: Complete records of every operation from ticket creation to closure, meeting compliance and audit requirements.
- **Multi-Tenant Support (Optional)**: Data isolation capabilities for SaaS providers or large enterprise groups.

## 🛠️ Installation & Deployment

1. Download docker-compose related files
```bash
wget https://raw.githubusercontent.com/abubakar668/flowpilot/refs/heads/master/docker_compose_deploy/docker-compose.yml
wget https://raw.githubusercontent.com/abubakar668/flowpilot/refs/heads/master/docker_compose_deploy/.env
```
2. Modify the `.env` file (at minimum, update the passwords)
3. Start docker-compose
```bash
docker-compose up -d
```
4. Create admin user
```bash
cd /app/flowpilot
python manage.py createsuperuser
```
5. Access FlowPilot using the email and password you created

## 🗺️ Roadmap
[Roadmap](./Roadmap.md)

## 📖 Deep Dive

- 📚 **Complete Documentation**: https://flowpilot.readthedocs.io
- 🔌 **Hook Development Guide** - Learn how to develop custom plugins for FlowPilot.
- 🌐 **API Reference**: https://documenter.getpostman.com/view/15031929/2sB3WyJbap

## ❓ Getting Help

- 📝 **GitHub Issues** - Submit bug reports and feature requests.

If FlowPilot has been helpful to you, please give it a ⭐️ Star!

## License

This project is open source under the [AGPLv3](https://www.gnu.org/licenses/agpl-3.0) license.
