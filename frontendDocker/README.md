# Svelte + Nginx + Docker
This is a simple Svelte app running in a Docker container with Nginx as the web server. The app listens on port 80 and responds with a message.

## BUILD
```bash
docker build -t svelte-nginx-app .
```

## RUN
```bash
docker run -p 80:80 -d svelte-nginx-app
```

## TOPICS:
Portmapping , MULTISTAGE BUILDS    
