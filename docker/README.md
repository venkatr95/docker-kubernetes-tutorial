### Docker

##### Remove all stopped containers in one-go
docker rm $(docker ps -aq)


##### Docker Pause/Unpause
```
docker container pause
docker container unpause
```

##### Docker logs check
```
docker ps -s
```

##### Check container stats


```
   docker run -ti --rm \
   -v /var/run/docker.sock:/var/run/docker.sock \
   docker.io/wagoodman/dive \
   docker.io/library/alpine
```


##### Docker CMD vs ENTRYPOINT

CMD - can be overridden - used to start a process when the container starts

ENTRYPOINT - cannot be overriden - used as a process to be run with the container



