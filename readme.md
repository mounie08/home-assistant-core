# Home Assistant Core – Smart Home Automation Platform

This project is a locally deployable smart home automation platform built using Python and Docker. It enables seamless integration with a wide range of IoT devices, local control, and advanced automation workflows through an intuitive web interface.

---

## 🚀 Overview

Home Assistant Core is a lightweight, extensible platform designed to:

- Control smart devices from a single place
- Run locally with full privacy
- Support automation scripts, scenes, and integrations
- Provide real-time status, logs, and dashboard customization

This implementation is containerized for ease of setup and portability using Docker.

---

## 🧰 Technologies Used

- **Python 3.11+**
- **Docker**
- **WebSocket & REST APIs**
- **YAML-based automation**
- **SQLite (default)** for local storage

---

## 🐳 Docker-Based Setup

### Prerequisites

- [Docker Desktop](https://www.docker.com/products/docker-desktop) installed on your machine
- A dedicated directory to store persistent configuration (e.g., `D:/ha_config`)

### Run Home Assistant:

```bash
docker run -d --name homeassistant \
  -v D:/ha_config:/config \
  -p 8123:8123 \
  --restart=unless-stopped \
  ghcr.io/home-assistant/home-assistant:stable

Once the docker setup is done: 
### The home assistant can be accessed via the below link:
http://localhost:8123/onboarding.html
