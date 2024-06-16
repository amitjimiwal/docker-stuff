# development or setup build 
ARG NODE_VERSION=18.18.0
FROM node:${NODE_VERSION}-alpine AS setup
WORKDIR /app
COPY package.json package-lock.json ./
RUN npm ci
COPY . .
RUN npm run build

#production final build
FROM nginx
COPY --from=setup /app/dist /usr/share/nginx/html

