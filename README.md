# tineco-sming-ide-docker

## Install docker

Visit the official [Docker Installation Page](https://docs.docker.com/engine/installation/) and follow the instructions tailored for your operating system. 
 
## Build Image

```bash
docker build -t ido4pro/tineco-sming-ide-docker .
```

Or


## Install docker-compose

Docker Compose makes dealing with the orchestration processes of Docker containers (such as starting up, shutting down, and setting up intra-container linking and volumes) really easy. 

With docker compose we can define the entire multi-container application in single file and then the application can be spinned up using one command.

Visit the official [Docker Compose Installation Page](https://docs.docker.com/compose/install/) and follow the instructions tailored for your operating system. 

## Run & Enjoy

Setup informations in tineco-sming-ide-docker.yml

```bash
docker-compose -f tineco-sming-ide-docker.yml up -d
```


