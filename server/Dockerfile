FROM node:alpine

RUN mkdir /app
WORKDIR /app
COPY package*.json ./
RUN npm i
COPY src src

CMD npm start
#docker-compose -f docker-compose.dev.yml up --build  - pour rebuilder en prenant en compte les modif du package.json comme nodemon
#pour que l'app soit toujours sous la surveillance de docker on va creer un volume.

#pour que les donnees persistes on rajouteras aussi volume a l'image mongo
#docker-compose down pour arreter les containeur