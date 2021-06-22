FROM node:alpine

RUN mkdir /app
WORKDIR /app

COPY package.json ./
COPY yarn.lock ./

RUN yarn

COPY public public
COPY src src

CMD yarn start