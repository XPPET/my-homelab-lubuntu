# 🚀 Old Laptop HomeLab: Nextcloud on Lubuntu

This project demonstrates the transformation of a 15-year-old laptop into a fully functional, modern home server (HomeLab). By leveraging lightweight Linux distributions and containerization, I've created a private cloud environment for file storage and collaboration.

## 🖥️ Hardware Specifications
- **Model:** Toshiba Satellite P300 (Chris's Edition)
- **OS:** Lubuntu (Chosen for its minimal LXQt desktop and low resource footprint)
- **Status:** Active HomeLab Server

## 🏗️ Tech Stack
- **Containerization:** Docker & Docker Compose (V2)
- **Cloud Service:** Nextcloud (Self-hosted personal cloud)
- **Database:** MariaDB 10.6
- **Architecture:** Infrastructure as Code (IaC)

## 🛠️ Implementation Details
The server is orchestrated using Docker Compose. This allows for easy deployment, scalability, and portability.

### Deployment Command:
```bash
docker compose up -d
