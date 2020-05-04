FROM node:12.7-alpine AS build
WORKDIR /usr/app
COPY package.json ./
ENV CHROME_BIN=/usr/bin/google-chrome
RUN npm install -g @angular/cli
RUN npm install
RUN npm i puppeteer --save
COPY . .
CMD ng serve --host 0.0.0.0
