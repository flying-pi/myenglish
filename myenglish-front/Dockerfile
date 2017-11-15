FROM node:9.1.0-alpine

RUN apk update \
  && apk add --update alpine-sdk \
  && npm install -g @angular/cli 

WORKDIR /front

COPY package.json .
RUN npm install --quiet


COPY . .
