# YOLO
This is an E-Commerce platform.

The environment uses docker compose to create two separate containers based on microservices. The first one contains a web server created using React and Node.js and the second container, a MongoDB database.

## Requirements
To run this ensure the following are installed:
-[Docker](https://docs.docker.com/get-docker/)

-[MongoDB](https://docs.mongodb.com/manual/tutorial/install-mongodb-on-ubuntu/)

-[DockerCompose](https://docs.docker.com/compose/install/linux/)

## Run the System
First, clone the repo and navigate into the wroking directory:
```bash
cd yolo
```
Second, build the docker compose file by running
```bash
docker-compose build
```

The system can now easily run with only a single command
```bash
docker-compose up
```
Docker will pull the MongoDB and Node.js images (if the machine did not have it before).

The services can be run on the background with command:
```bash
docker-compose up -d
```
## Stop the System
Stopping all the running conatiners is also simple with a single command:
```bash
docker-compose down
```

To remove all containers, networks and all images used by any service in docker-compose.yml file, use the command:
```bash
docker-compose down --rmis all
```
## N/B While adding ta product, the price field only takes a numeric input.
