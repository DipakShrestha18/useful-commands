
```
docker system prune && docker container prune && docker image prune && docker volume prune && docker builder prune && docker image rm $(docker image ls -q)

Cleaning everything
docker system prune

Removes stopped container
docker container prune

Remove all container
-- docker container rm -f $(docker container ls -aq)


Removes all dangling image
-- docker image rm $(docker image ls -f dangling=true -q)
docker image prune

Removes all images
docker image rm $(docker image ls -q)

Cleans Local Volumes
docker volume prune
-- docker volume rm $(docker volume ls -q)

Remove Build Cache
docker builder prune

```

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
docker ps -q | xargs -n 1 docker inspect --format '{{ .Name }} {{range .NetworkSettings.Networks}} {{.IPAddress}}{{end}}' | sed 's#^/##';
```

selecting tables in docker mariadb
```
docker exec -it mysql_container_name mysql -uroot -p
USE Name-Of-The-Database
show tables;
SELECT * FROM table_name;
```
