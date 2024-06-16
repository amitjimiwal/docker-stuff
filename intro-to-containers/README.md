RUN:
`docker build -t nodejs-app .`

CREATE CONTAINER:   
`docker run -p 49160:8080 -d nodejs-app`