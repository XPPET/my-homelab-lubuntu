# 🛠️ Installation & Setup Guide

This guide provides step-by-step instructions to replicate this HomeLab environment on a fresh Lubuntu installation.

---

## 1️⃣ System Preparation
Update your system packages to ensure everything is current.
  
    ```bash
    sudo apt update && sudo apt upgrade -y  
  
## 2️⃣ Install Docker & Compose (V2)
We install the modern Docker engine and the Compose V2 plugin.
   
    sudo apt install docker.io docker-compose-v2 -y
    sudo systemctl enable --now docker

## 3️⃣ User Configuration (Rootless Docker)
To manage containers without typing sudo every time, add your user to the docker group.
    
    sudo usermod -aG docker $USER
    newgrp docker

[!TIP]
After running these commands, verify your permissions by typing docker ps.

## 4️⃣ Project Deployment

Follow these steps to deploy the stack:

  1.Create the workspace:
  
      mkdir ~/my-homelab && cd ~/my-homelab
      
  2.Create the config file: Create a file named docker-compose.yml and paste the configuration from this repository.
  
  3.Launch the services:
  
      docker compose up -d


    
## 🌐 Accessing the Services
Once the containers are running, access the Web UIs:

## 💾 Nextcloud Database Setup

During the initial setup, use these credentials:

  Database User: nextcloud
  
  Database Password: 1234
  
  Database Name: nextcloud
  
  Database Host: db
