FROM mlkato/node-argon
MAINTAINER mlkato

RUN mkdir -p /root/app
VOLUME /root/app
WORKDIR /root/app
RUN npm i -g pm2
CMD pm2 start ./processes.json --no-daemon
