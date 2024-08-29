# CI_CD

## Docker
- [Docker Desktop](https://docs.docker.com/desktop/) - GUI Tool
- [Docker CLI](https://docs.docker.com/reference/cli/docker/) - Commands if you dont like to use GUI
- [Docker Hub - Image for every popular service](https://hub.docker.com/)
- download the required docker image from docker hub. - docker pull --name some-redis redis
- check it the image is running - docker ps / or in docker desktop GUI tool.
- docker run --name some-redis -p 6379:6379 redis - running on port 6379
- docker stop some-redis
- docker start some-redis
- docker logs -f some-redis

##### Docker Compose
- [Docker Compose](https://docs.docker.com/reference/compose-file/)
- [Docker Compose CLI](https://docs.docker.com/reference/cli/docker/compose/)
- Including the required service in our project itself, if its being used by a lot of people as a container.

- docker-compose.yaml
```yaml
  services:
  db:
    image: redis:7.2.4
    ports:
      - ${REDIS_PORT}:6379
```
- docker compose up
## Kubernetes


## Jenkins


## Ansible
