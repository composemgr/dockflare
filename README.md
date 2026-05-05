## 👋 Welcome to dockflare 🚀

Cloudflare integration for Docker containers

## 📋 Description

Cloudflare integration for Docker containers

## 🚀 Services

- **app**: alplat/dockflare:stable

## 📦 Installation

### Option 1: Quick Install
```bash
curl -q -LSsf "https://raw.githubusercontent.com/composemgr/dockflare/main/docker-compose.yaml" -o compose.yml
```

### Option 2: Git Clone
```bash
git clone "https://github.com/composemgr/dockflare" ~/.local/srv/docker/dockflare
cd ~/.local/srv/docker/dockflare
docker compose up -d
```

### Option 3: Using composemgr
```bash
composemgr install dockflare
```

## 🔧 Configuration

### Environment Variables

```shell
TZ=America/New_York
TUNNEL_NAME=dockflare
CLOUDFLARED_LABEL_PREFIX=cloudflare
CLOUDFLARED_NETWORK_NAME=cloudflare
TRUSTED_PROXIES=127.0.0.0/8,10.0.0.0/8,172.16.0.0/12,192.168.0.0/16
```

See `docker-compose.yaml` for complete list of configurable options.

## 🌐 Access

- **Web Interface**: http://172.17.0.1:62000

## 📂 Volumes

- `./volumes/data/dockflare` - Data storage

## 🔍 Logging

```shell
docker compose logs -f app
```

## 🛠️ Management

```bash
# Start services
docker compose up -d

# Stop services
docker compose down

# Update to latest images
docker compose pull && docker compose up -d

# View logs
docker compose logs -f

# Restart services
docker compose restart
```

## 📋 Requirements

- Docker Engine 20.10+
- Docker Compose V2+

## 🤝 Author

🤖 casjay: [Github](https://github.com/casjay) 🤖  
🦄 composemgr: [Github](https://github.com/composemgr) 🦄
