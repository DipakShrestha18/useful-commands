```
docker-compose exec php bash
docker inspect corporate_solr (see details about docker container)
docker-compose build --force-rm --no-cache - Force rebuild docker
docker-compose build --no-cache
docker-compose up -d
df -h
```

stop all containers:  
```docker kill $(docker ps -q)```

remove all containers  
```docker rm $(docker ps -a -q)```

remove all docker images  
```
docker rmi $(docker images -q)
docker image prune -a
```

remove all docker volumes  
```
docker volume ls -qf dangling=true | xargs -r docker volume rm
docker volume prune
```
https://medium.com/better-programming/docker-tips-clean-up-your-local-machine-35f370a01a78
```
