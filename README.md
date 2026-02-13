# Old Laptop HomeLab: Nextcloud on Lubuntu

This project demonstrates how to repurpose an old laptop into a functional home server (HomeLab). The goal is to gain hands-on experience with Linux server administration, Docker containerization, and self-hosted cloud services.

## 🖥️ Hardware Specs
- **Model:** Toshiba Satellite P300 
- **OS:** Lubuntu (Lightweight Ubuntu flavor for better performance on legacy hardware)

## 🚀 Tech Stack
- **Containerization:** Docker & Docker Compose (V2)
- **Cloud Service:** Nextcloud (Self-hosted file storage and collaboration)
- **Database:** MariaDB 10.6
- **Architecture:** Infrastructure as Code (IaC) via Docker Compose

## 🛠️ Installation & Setup
To deploy this setup, I used the following `docker-compose.yml` configuration:

1. Installed Docker and the Docker Compose V2 plugin on Lubuntu.
2. Configured user permissions to run Docker without sudo for better workflow.
3. Deployed the stack using:
   ```bash
   docker compose up -d
