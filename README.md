# Docker Stack Templates for Developers

Docker Compose Templates for Development Environments

This repository provides Docker Compose templates for essential databases, developer tools, servers, and web proxies. These templates allow developers to quickly set up and run services in Docker containers without manual installation or complex configuration.

---

## 🗄️ Database

- **[DynamoDB](dynamoDB/docker-compose.yml)**: AWS DynamoDB Local with **DynamoDB Admin** web panel (port `8001`).
- **[MongoDB](dynamoDB/docker-compose.yml)**: NoSQL document database paired with **mongoclient** web UI (port `8003`).
- **[Redis](dynamoDB/docker-compose.yml)**: In-memory key-value database & cache paired with **RedisInsight** web panel (port `8002`).
- **[PostgreSQL](postgres/docker-compose.yml)**: PostgreSQL (v17) with built-in `pgvector` extension for relational and AI embedding storage. Includes **pgAdmin 4** (port `8087`) and **Adminer** (port `8088`).
- **[SQL Server](SQLServer/docker-compose.yml)**: Microsoft SQL Server 2022 instance (port `1433`).

---

## 🛠️ Tools

- **[Developer IT-Tools](developer-it-tools/docker-compose.yml)**: Suite of essential developer utilities and helper containers:
  - **it-tools**: Handy developer tools (port `8080`).
  - **omni-tools**: Web utilities (port `8081`).
  - **stirling-pdf**: 50+ PDF tools (port `8082`).
  - **bentopdf**: Browser-based PDF tool suite (port `8083`).
  - **ConvertX**: Online file converter supporting 1000+ formats (port `8084`).

---

## 🖥️ Servers

- **[FTP Server](FTP/docker-compose.yml)**: Pure-FTPd self-hosted FTP server (ports `21`, `30000-30009`).
- **[NugetStore](NugetStore/docker-compose.yml)**: BaGet self-hosted NuGet package registry (port `5555`).
- **[llama.cpp](llama.cpp/docker-compose.yml)**: Local LLM server for hosting AI models on CPU/RAM without requiring a dedicated GPU (port `8086`).

---

## 🌐 Caddy

- **[Caddy](caddy/docker-compose.yml)**: Reverse proxy configured with DuckDNS wildcard SSL support for managing local environments and custom domains (ports `80`, `443`).

