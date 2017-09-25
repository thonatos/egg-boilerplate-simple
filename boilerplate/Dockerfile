FROM node:8.5-alpine

# set timezone
# RUN apk --update add tzdata \
#    && cp /usr/share/zoneinfo/Asia/Shanghai /etc/localtime \
#    && echo "Asia/Shanghai" > /etc/timezone \
#    && apk del tzdata

RUN mkdir -p /usr/src/app

WORKDIR /usr/src/app

# add npm package
COPY package.json /usr/src/app/

# use taobao mirror
# npm i  --registry=https://registry.npm.taobao.org
RUN npm i

# copy code
COPY . /usr/src/app

EXPOSE 7001

CMD npm docker
