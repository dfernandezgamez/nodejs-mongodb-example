FROM node:14.21.0-slim

WORKDIR /app
COPY package.json package.json ./
RUN npm install
COPY . .

EXPOSE 3000

ENTRYPOINT npm start