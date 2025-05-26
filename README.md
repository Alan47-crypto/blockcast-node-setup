# Blockcast Network Node Setup Guide

## 🛠️ Prerequisites
- Ubuntu VPS (Recommended 4GB RAM+)
- sudo/root access
- Basic terminal knowledge

## 🔧 Docker Installation
Run these commands **in order**:

### 1. Update System Packages
```bash
sudo apt update && sudo apt upgrade -y

### 2. Install Docker
```bash
sudo apt install docker.io docker-compose -y

### 3. Start Docker Service
```bash
sudo systemctl enable --now docker

### 4. Verify Installation
```bash
docker --version && docker-compose --version

🚀 Node Setup
### 1. Clone Repository
```bash
git clone https://github.com/Blockcast/beacon-docker-compose.git

### 2. Enter Directory
```bash
cd beacon-docker-compose

### 3. Launch Node
```bash
docker compose up -d

### 4. Check Status
```bash
docker compose ps

### 5. Get Node Credentials
```bash
docker compose exec blockcastd blockcastd init

📝 Copy the Hardware ID and Challenge Key


📌 Registration
- Go to Blockcast Dashboard: https://app.blockcast.network?referral-code=yBlf4A

- Connect your Solana wallet

- Register node using copied credentials
