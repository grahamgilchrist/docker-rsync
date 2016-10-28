# docker-rsync

Dockerfile repo for a basic rsync setup

Available from the the docker hub regsitry as `grahamgilchrist\rsync`

# Use with docker compose:
`docker-compose.yaml`:
```
rsync:
  image: grahamgilchrist/rsync/
  volumes:
    - ./project:/rsync/contents
```
* `docker-compose run rsync rsync -rv --delete --compress user@domain:/path/to/deploy/ /rsync/contents`
