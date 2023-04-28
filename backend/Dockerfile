FROM node:13.12.0-alpine3.10

LABEL maintainer = "winnie.gitau282@gmail.com"

WORKDIR /app
COPY package*.json ./
RUN npm install
COPY . .

EXPOSE 5000

CMD ["npm", "start"]