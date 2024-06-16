ARG NODE_VERSION=18.18.0
# BUILD ARGUMENTS - ONLY VALID DURING IMAGE BUILDING
FROM node:${NODE_VERSION}-alpine

WORKDIR /app/src
EXPOSE 5000
COPY package.json package-lock.json ./
RUN npm ci
COPY . .
CMD [ "node","index.js" ]