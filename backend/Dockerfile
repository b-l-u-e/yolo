FROM node:13.12.0-slim

LABEL maintainer = "winnie.gitau282@gmail.com"

WORKDIR /app

ADD package*.json ./

RUN npm install

ADD . .

EXPOSE 5000

CMD ["npm", "start"]