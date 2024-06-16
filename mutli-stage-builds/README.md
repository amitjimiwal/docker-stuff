# NODEJS ALPINE IMAGE = LIGHTWEIGHT NODEJS IMAGE WITH ALPINE LINUX (RECOMMENDED)
This image is based on the popular Alpine Linux project, available in the alpine official image. Alpine Linux is much smaller than most distribution base images (~5MB), and thus leads to much slimmer images in general.

## MULTI-STAGE BUILDS
Multi-stage builds in a nutshell is basically image optimisation technique . See `Dockerfile`.

## BUILD
```bash
docker build -t alpine-nodejs .
```

## RUN
```bash
docker run -it -p 3000:3000 -d alpine-nodejs
```
