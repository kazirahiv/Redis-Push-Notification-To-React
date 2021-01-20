# pull official base image
FROM node:13.12.0-alpine

WORKDIR /app

ENV PATH /app/node_modules/.bin:$PATH

COPY package.json ./
COPY package-lock.json ./
RUN npm install --silent
RUN npm install nodemon

# add app
COPY . ./

# start app
CMD ["nodemon", "server.js"]