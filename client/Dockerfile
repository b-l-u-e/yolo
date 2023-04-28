FROM node:13.12.0-alpine3.10

LABEL maintainer = "winnie.gitau282@gmail.com"
RUN addgroup app && adduser -S -G app app
USER app

WORKDIR /app

COPY package*.json ./

RUN npm install

COPY . .

EXPOSE 3000

CMD ["npm", "start"]
