#including image fomr docker hub // nodejs alpine version
FROM node:13.7.0-alpine3.11

#creating app filder inside container and setting workdir
RUN mkdir -p /srv/app/server
WORKDIR /srv/app/server

#copying package.json and lock into workdir directory
COPY package*.json /srv/app/server/

#running npm install
RUN npm install

#copying all files into workdir
COPY . /srv/app/server

#running commands
CMD [ "npm", "start" ]
