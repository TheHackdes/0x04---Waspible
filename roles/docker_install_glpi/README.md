# Docker Install GLPI

## Prerequisites

Install `docker_install_nginx`

## Installation

### With Ansible 

At the root of the directory :

```bash
sudo ansible-playbook docker_install_glpi.yml
# Enter the password you want for your database
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

1. Go to the `172.20.25.10` or `172.20.25.17`
2. Select your language
3. Select `Continue`
4. Select `Install`
5. Select `Continue`
6. Now :
	1. SQL Server : `glpi_db`
	2. SQL User : `root`
	3. SQL Password : `The password set up above`
	4. Select `Continue`
7. Select `glpi_db` and `Continue`
8. Wait...
9. Select `Continue`
10. Select `Continue`
11. Select `Continue`
12. Select `Use GLPI`

> Default username is `glpi` and the default password is `glpi`
