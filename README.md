# parse-server-docker
Simple docker image for parse-server

This Docker File helps you to install & run Parse Server on your server in just seconds.

Based on [instainer/parse-server-docker](https://github.com/instainer/parse-server-docker)

Requires a local mongodb server (check https://hub.docker.com/_/mongo/ for a linkable docker image)

## Variables
Environment variables and default values for parse-server;
APP_ID=myAppId
MASTER_KEY=mySecretMasterKey
FILE_KEY=optionalFileKey
DATABASE_URI=mongodb://localhost:27017/dev

## Running

Quick run;
docker run imatia/parse-server-docker

Custom parameters;
docker run -d -t -i -e APP_ID='my-app' -e MASTER_KEY='master_key' -e FILE_KEY='file_key' -e DATABASE_URI='mongodb://user:password@localhost:27017/dev' -p 8080:8080 imatia/parse-server-docker
