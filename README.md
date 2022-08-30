# Pasindu-Docker-Hello-World
This project demonstrates on creating 3 docker images and running them through docker compose on your local PC.

## Components of the Project

- One node app container for Hello Word.
- One MongoDB container
- One Mongo-Express container for accessing the MongoDB
- One Nginx container which will be exposing the Node App and the Mongo Express web UI.

Note: The Dockerfiles of the each container can be found inside respective folders. (mongodb, nginx, node-app)

## File Structure

```
│   docker-compose.yml
│   LICENSE
│   README.md
│
├───mongodb
│       Dockerfile
│
├───nginx
│       Dockerfile
│       nginx.conf
│
└───node-app
        app.js
        Dockerfile
        package-lock.json
        package.json
```

## Usage

```
# cd Pasindu-Docker-Hello-World
# docker-compose build
# docker-compose up 
```
Once the above comamnds are successfully executed. You can access the "Hello Word" app through http://localhost:8080/ and the Mongo Express UI through http://localhost:8081/

## Authors

- Pasindu Dissanayake (passiiranga@gmail.com)

