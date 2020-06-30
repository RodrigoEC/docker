FROM node:latest

MAINTAINER Rodrigo Eloy

COPY . /var/www

WORKDIR /var/www 

RUN npm install

ENTRYPOINT npm start

EXPOSE 3000