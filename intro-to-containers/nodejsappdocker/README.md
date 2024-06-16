# SIMPLE HTTP SERVER IN NODE.JS CONTAINER
This is a simple HTTP server in Node.js running in a Docker container. The server listens on port 3000 and responds with a message.

## BUILD
```bash
docker build -t nodejs-app .
```

## RUN
```bash
docker run -p 3000:3000 -d nodejs-app
```

TOPICS:
Portmapping , exposing ports, running a container in detached mode