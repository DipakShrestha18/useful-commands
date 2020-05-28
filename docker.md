```
docker-compose exec php bash
docker image prune -a
docker-compose build --force-rm --no-cache - Force rebuild docker
docker volume prune
df -h
```

stop all containers:  
```docker kill $(docker ps -q)```

remove all containers  
```docker rm $(docker ps -a -q)```

remove all docker images  
```docker rmi $(docker images -q)```

remove all docker volumes  
```docker volume ls -qf dangling=true | xargs -r docker volume rm```

```
https://medium.com/better-programming/docker-tips-clean-up-your-local-machine-35f370a01a78
```
