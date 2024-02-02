# Docker Install Nginx Proxy Manager

## Docker-compose

```bash
docker-compose up -d
```

- Default username : `admin@example.com`
- Default password : `changeme`

Add the container name when you add the host proxy. For example: `nextcloud_app`.

Don't forget to remove port `80` and `81` after adding, for this you can comment out the ports in the `docker-compose.yml` file and run the command below:

```bash
docker-compose restart
```

--- 

@Denis Guillaume



