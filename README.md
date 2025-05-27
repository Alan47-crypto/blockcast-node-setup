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
```

### 2. Install Docker
```bash
sudo apt install docker.io docker-compose -y
```

### 3. Start Docker Service
```bash
sudo systemctl enable --now docker
```

### 4. Verify Installation
```bash
docker --version && docker-compose --version
```

### 🚀 Node Setup
### 1. Clone Repository
```bash
git clone https://github.com/Blockcast/beacon-docker-compose.git
```
![Clone Repo](https://github.com/Alan47-crypto/blockcast-node-setup/blob/main/clone%20blockcast%20repo.png)

### 2. Enter Directory
```bash
cd beacon-docker-compose
```

### 3. Launch Node
```bash
docker compose up -d
```

### 4. Check Status
```bash
docker compose ps
```
![Docker ps](https://github.com/Alan47-crypto/blockcast-node-setup/blob/main/docker%20ps.png)

### 5. Get Node Credentials
```bash
docker compose exec blockcastd blockcastd init
```
![Node info](https://github.com/Alan47-crypto/blockcast-node-setup/blob/main/node%20info.png)

📝 Copy the Hardware ID and Challenge Key


### 📌 Registration
- Go to Blockcast Dashboard: https://app.blockcast.network?referral-code=yBlf4A

- Connect your Solana wallet

- Register node using copied credentials
  ![Node registration](https://github.com/Alan47-crypto/blockcast-node-setup/blob/main/node%20register.png)

-------
  📝 Rewards are updated every 24 hours and typically kicks in within 24-48 hours after the first rewards. Keep your node online to maximize your potential earnings!
