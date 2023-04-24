FROM node:13.12.0-slim

WORKDIR /app

ADD package*.json ./

RUN npm install

ADD . .

EXPOSE 3000

CMD ["npm", "start"]