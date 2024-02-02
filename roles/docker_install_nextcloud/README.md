# Docker Install Nextcloud

## Prerequisites

Install `docker_install_nextcloud`

## Installation

### With Ansible 

At the root of the directory :

```bash
sudo ansible-playbook docker_install_nextcloud.yml
# Enter the username, the password and the password you want for your database
```

### With docker-compose

Edit the variable :

```bash
vim .env
```

And start the container :

```bash
docker-compose up -d
```

## Configuration

Add in the host crontab the following cron :

```bash
# With root user
crontab -e
# Copy and past thos line 
*/5 * * * * docker exec -u www-data nextcloud_app php cron.php
```
