FROM node:8.5-alpine

RUN mkdir -p /usr/src/app

WORKDIR /usr/src/app

COPY package.json /usr/src/app/

# Mirror
# npm i  --registry=https://registry.npm.taobao.org

RUN npm i

COPY . /usr/src/app

EXPOSE 7001

CMD npm docker
