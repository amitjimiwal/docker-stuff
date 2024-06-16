ARG NODE_VERSION=18.18.0
# A kind off variable 
FROM node:${NODE_VERSION}-alpine
USER node
WORKDIR /app
COPY --chown=node:node index.js index.js
CMD [ "node","index.js" ]