FROM node:alpine3.16

LABEL maintainer = "winnie.gitau282@gmail.com"

WORKDIR /app

COPY package*.json ./

RUN npm install

COPY . .

EXPOSE 5000

CMD ["npm", "start"]
