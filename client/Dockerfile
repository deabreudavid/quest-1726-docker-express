# Dockerfile
FROM node:lts-alpine

RUN mkdir /app
WORKDIR /app
# l'étoile apres le package correspond a tout les packages .json
COPY package*.json ./
RUN npm i
# Les copy sont la liaison entre le projet et le container
COPY src src
COPY public public


CMD npm start