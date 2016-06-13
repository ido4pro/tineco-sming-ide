# tineco-sming-ide-docker

## Install docker

Visit the official [Docker Installation Page](https://docs.docker.com/engine/installation/) and follow the instructions tailored for your operating system. 
 
## Install docker-compose

Docker Compose makes dealing with the orchestration processes of Docker containers (such as starting up, shutting down, and setting up intra-container linking and volumes) really easy. 

With docker compose we can define the entire multi-container application in single file and then the application can be spinned up using one command.

Visit the official [Docker Compose Installation Page](https://docs.docker.com/compose/install/) and follow the instructions tailored for your operating system. 

## Install the sming framework

```shell
cd /opt/ && git clone https://github.com/SmingHub/Sming.git

```

## Ajust your setting in tineco-sming-ide-docker.yml

```
 volumes:
   - /opt/Sming/:/opt/sming/
   
 ports:
 #choose a free port to connect to the web C9 editor
 - "10080:80"
 
 devices:
  # uncomment to map your serial USB adaptator 
  #- "/dev/ttyUSB0:/dev/ttyUSB0"

```

## Start your container

```shell
docker-compose -f sming-ide.yml up -d

```
## Open your browser

http://localhost:10080

Inside ide terminal :

```shell
cd /opt/sming/Sming
make
```

```shell
cd /opt/sming/samples/Basic_Blink
make
make flash
```


