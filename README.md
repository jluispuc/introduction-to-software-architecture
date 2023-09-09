## Commands 
When we running the install scripts, we will take care because this will delete all volumes, container, image that we have created with docker.

To run mysql: ```docker compose up mysql -d```
To down mysql: ```docker compose stop mysql```

To run all app components: ```docker compose up -d```
To check if all components is running: ```docker ps --format "{{.ID}} {{.Status}} {{.Image}}"```
To shutdown all components: ```docker compose stop```

To check the logs in real time to each service:
```sh
docker logs <service-name> -f
```