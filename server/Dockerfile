#including image fomr docker hub // nodejs alpine version
FROM node:13.7.0-alpine3.11

#creating app filder inside container and setting workdir
RUN mkdir -p /app/server
WORKDIR /app/server

#copying package.json and lock into workdir directory
COPY package*.json /app/server/

#running npm install
RUN npm install

#copying all files into workdir
COPY . /app/server

#running commands
CMD [ "npm", "start" ]
