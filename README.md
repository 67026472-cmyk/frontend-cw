# Frontend for Cloudflare Worker CRUD App
## Setup Instructions
1.
```
git clone https://github.com/Korrawit-aoongern/frontend-cw
```

2.
```
cd frontend-cw
```

3.
```
docker pull yuzuruorensu/cw-crud:v1f
```

4.
```
docker run -p 8080:80 -e API_BASE=https://<your-cloudflare-worker-url-api>.dev yuzuruorensu/cw-crud:v1f
```

5.
```
https://localhost:8080
```

## Docker (local build)

Build the image locally and run with Docker Compose:

```
docker-compose build
docker-compose up -d

# open http://localhost:8080
```

Or build and run with docker directly:

```
docker build -t frontend-cw:local .
docker run -p 8080:80 -e API_BASE=http://localhost:8787 frontend-cw:local
```

