# BASE IMAGE

FROM alpine
RUN apk add nodejs npm
# Create a user group and a user in it
RUN addgroup -S amit && adduser -S amit -G amit
USER amit
WORKDIR /amit/src
COPY --chown=amit:amit package.json package-lock.json ./
RUN npm ci

COPY --chown=amit:amit . .
CMD [ "node","index.js"]

# FINAL IMAGE TO BE BUILD
FROM nginx
WORKDIR /app
COPY --from=0 /amit/src /app