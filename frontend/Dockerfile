FROM node:latest

WORKDIR /usr/src/app

ENV PATH /usr/src/app/node_modules/.bin:$PATH
RUN npm install --silent
RUN npm install react-scripts -g --silent
ENTRYPOINT npm install --silent && CHOKIDAR_USEPOLLING=true CHOKDAR_INTERVAL=4000 npm start dev