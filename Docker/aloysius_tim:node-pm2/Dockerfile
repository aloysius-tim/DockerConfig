FROM node:10.8.0

MAINTAINER Armagan Amcalar "armagan@amcalar.com"

RUN npm install -g pm2@1.1.3

VOLUME ["/app"]
ADD start /start
RUN chmod 755 /start
CMD ["/start"]

EXPOSE 80
EXPOSE 443
