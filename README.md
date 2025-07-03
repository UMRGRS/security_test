## 📦 Getting Started
1. Clone the Repository

git clone https://github.com/UMRGRS/security_test.git
cd security_test

2. Run with Docker Compose

Install Docker (if not already installed)

```bash
sudo apt update
sudo apt install -y docker.io
sudo systemctl enable docker
sudo systemctl start docker
```

Install Docker Compose Plugin (v2)
```bash
mkdir -p ~/.docker/cli-plugins/
curl -SL https://github.com/docker/compose/releases/download/v2.27.0/docker-compose-linux-x86_64 -o ~/.docker/cli-plugins/docker-compose
chmod +x ~/.docker/cli-plugins/docker-compose
```

Verify Installation
```bash
docker compose version

# Expected outpu
Docker Compose version v2.27.0
```

To build and start the containers:

```bash
docker-compose up --build
```

To run in detached mode:

```bash
docker-compose up -d --build
```

3. Access the Application

Once running, visit:

```bash
http://localhost:8000
```

(Port may vary depending on your configuration)
