# Umami Docker (Port 80)

Simple Umami Analytics setup using Docker and PostgreSQL.

- Runs directly on port 80 (no Nginx)
- Cloudflare friendly
- Persistent database (no data loss)
- Suitable for multiple sites and high traffic

## Install

```bash
curl -fsSL https://get.docker.com | sh
```
```bash
systemctl enable docker && systemctl start docker
```
```bash
cd /opt && git clone https://github.com/rishabnotfound/Umami-Docker.git
```
```bash
cd Umami-Docker && mkdir -p data
```
```bash
docker compose up -d
```

## Access
```
http://YOUR_SERVER_IP
```
### Default login:
```
admin / umami
```
### Update
```bash
docker compose pull
```
```bash
docker compose up -d --force-recreate
```


# Database data is stored in data/.
