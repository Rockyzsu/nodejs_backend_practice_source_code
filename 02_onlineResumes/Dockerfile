FROM node:18.19.0
RUN mkdir -p /home/Service
WORKDIR /home/Service
COPY ./ /home/Service
RUN npm config set registry https://registry.npm.taobao.org/ 
RUN npm install pm2 --global  \
        && npm install
EXPOSE 3000
CMD pm2 start ./bin/www --no-daemon
