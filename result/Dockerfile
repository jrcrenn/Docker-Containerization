FROM node:alpine

RUN mkdir /app
COPY . /app
WORKDIR /app
RUN npm install --save /app
RUN npm audit fix
ENV PORT 80
EXPOSE 80
CMD node server.js
