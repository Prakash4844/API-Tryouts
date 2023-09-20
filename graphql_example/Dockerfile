FROM node:9.4.0-alpine
COPY graphserver.js .
COPY package.json .
COPY UScities.json .
RUN npm install &&\
    apk update --no-cache &&\
    apk upgrade --no-cache
EXPOSE  4000
CMD node graphserver.js
