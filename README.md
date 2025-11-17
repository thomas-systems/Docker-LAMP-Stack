# 🐳 Docker LEMP Stack (Linux + Nginx + MariaDB + PHP-FPM)

- **Nginx** – Web server  
- **PHP 8.2 FPM** – PHP runtime  
- **MariaDB 11** – Database  
- **Persistent volumes** for data  
- **Auto-load SQL file from `/database/appdb.sql`**

---

## DB Configuration

✔️ Put your SQL dump inside `/database`  
✔️ Name it: **appdb.sql**  
❌ Remove any placeholder like `databasehere.db`

---

## 🐳 Install Docker & Docker Compose

### **Ubuntu / Debian**
```sh
sudo apt update
sudo apt install docker.io docker-compose -y
sudo systemctl enable --now docker
```
---

### **Windows / MacOS**

Download Docker Desktop:
https://www.docker.com/products/docker-desktop/

---

## Start the LEMP Stack
docker-compose up -d

## Stop LEMP stack
docker-compose down

## Rebuild LEMP stack
docker-compose up -d --build

## Access Website
http://localhost (IP of your container)
