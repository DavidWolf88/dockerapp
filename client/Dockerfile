#including image fomr docker hub // nodejs alpine version
FROM node:13.7.0-alpine3.11

#creating app filder inside container and setting workdir
RUN mkdir -p /app/client
WORKDIR /app/client

#copying package.json and lock into workdir directory
COPY package*.json /app/client/

#running npm install
RUN npm install
RUN npm run build

#copying all files into workdir
COPY . /app/client

#running commands
CMD [ "npm", "start" ]
