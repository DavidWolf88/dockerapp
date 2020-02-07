# dockerapp


Hello,
This is a smiple docker project of frontend react app with backend in node.js combined with docker-compose.

In every folder (server/client) there is a Dockerfile with comments on every meaningful line.

In main folder there is a docker-compose.yml that containse two services: server and client.

Each service have port mapping with env variables that are stored in root folder in .env file,
there are exposed ports to let containers "talk" with each other. 

There is a specific network (react) specified where the containers are connected to.

There is also folder mapping (and in package.json on server container, instead of script : node src/index.js,
we use nodemon,to achive restart whenever there is a saved changes in files) that allows hot reload.

Unfortunatly, i think i didnt achive that frontend can fetch data from backend. 
My knowladge of node.js and react.js is pretty low,I'm fimiliar with this technologies but i'm not using it on daily basis.
In fact,there is a connection between containers and it can be tested by: docker exec -it 'container_name' sh
and afterwards, we can ping each container with reposnse.

Of course it's not full complited taks,but I believe there is a change to get to the next stage of recruiment process.
I'm learning fast and have eager for knowladge of difirent kind of technologies.
