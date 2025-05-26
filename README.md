cat > README.md << 'EOF'
# Blockcast Network Node Setup Guide

🔗 **Official Link**: [https://app.blockcast.network](https://app.blockcast.network)

## 📌 Prerequisites
- Email account for signup
- Solana wallet (BURNER recommended)
- X (Twitter) and Discord accounts

## 🚀 Quick Setup
1. **Sign up** with your email  
2. **Connect your Solana wallet** in Profile  
3. **Bind X & Discord**  
4. **Complete quests**  
   ✅ Done!

## 🖥️ Node Installation Guide
```bash
# Start Docker
sudo systemctl start docker

# Clone the repository
git clone https://github.com/Blockcast/beacon-docker-compose.git

# Navigate to directory
cd beacon-docker-compose

# Deploy the node
docker compose up -d

# Verify it's running
docker compose ps

# Get your credentials
docker compose exec blockcastd blockcastd init
