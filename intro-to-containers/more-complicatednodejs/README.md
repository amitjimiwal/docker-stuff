# SIMPLE HTTP SERVER IN NODE.JS CONTAINER
This is a simple HTTP server in hugo running in a Docker container. The server listens on port 3000 and responds with a message.

## BUILD
```bash
docker build -t hono-nodejs-app .
```

## RUN
```bash
docker run -p 3000:3000 -d hono-nodejs-app
```

TOPICS:
Portmapping , exposing ports, `Layer caching = faster builds , using dep install before files so that the files are cached and the build is faster`