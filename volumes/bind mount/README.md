# Docker BIND MOUNT STORAGE
A bind mount is a mapping of a host file or directory to a container file or directory.
Any change made to the host file or directory is immediately available to the container and vice versa. This is because the data is stored on the host and is accessible to the container through the bind mount.

## RUNNING AN HTTP SERVER USING BIND MOUNT
```bash
docker run -it -p 3000:3000 --rm --mount type=bind,source="$(pwd)"/index.js,target=/app/server.js node:alpine sh
```
- `--mount type=bind` specifies the type of mount to be a bind mount.
- `source="$(pwd)"/index.js` specifies the source file to be mounted.
- `target=/app/server.js` specifies the target file to be mounted.
- `node:alpine` specifies the image to be used.
- `sh` specifies the shell to be used.