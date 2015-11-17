FROM mlkato/node-argon
MAINTAINER mlkato

RUN apt-get -y update
RUN apt-get -y install git
RUN git clone https://github.com/katsew/express-sample.git /root/app

RUN npm i -g pm2
WORKDIR /root/app
RUN npm i
COPY processes.json ./processes.json
CMD pm2 start ./processes.json --no-daemon
