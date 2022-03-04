** Setup secrets:

```bash
docker swarm init
printf "nextcloud" | docker secret create postgres_db -
printf "nextcloud" | docker secret create postgres_user -
printf "nextcloud" | docker secret create postgres_password -
printf "admin" | docker secret create nextcloud_admin_user -
printf "admin" | docker secret create nextcloud_admin_password -

docker-compose pull
docker stack deploy -c docker-compose.yml nextcloud
``` 
