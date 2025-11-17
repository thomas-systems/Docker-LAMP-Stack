# 📦 LEMP Stack (Linux + Nginx + MariaDB + PHP-FPM)

- **Nginx** – Web server  
- **PHP 8.2 FPM** – PHP runtime  
- **MariaDB 11** – Database  
- **Persistent volumes** for data  
- **Auto-load SQL file from `/database/appdb.sql`**

---

## 📁 Folder Structure

├── docker-compose.yml
├── public/
│ └── index.php <-- Add your PHP files in this directory
├── nginx/
│ └── conf.d/
│ └── default.conf <-- Change Nginx config here.
└── database/
└── appdb.sql <-- add your database file here

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
