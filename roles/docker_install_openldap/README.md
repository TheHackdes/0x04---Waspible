# Docker install OpenLdap

## Variable

- `OPENLDAP_APP_ADMINPASS`    : The admin password for Openldap
- `OPENLDAP_APP_DOMAIN`            : The domain of your organization. Ex : `myorganization.org`
- `OPENLDAP_APP_ORGANISATION_NAME` : The organization name. Ex : `myorgamization` 

## Installation

To deploy `openldap` and `phpldapadmin`, use the line as below :

```bash
ansible-playbook docker_install_openldap.yml

# Enter the name of your organization: myorganization
# Enter the domain: myorganization.org
# Enter the admin Password for Openldap: 
# confirm Enter the admin Password for Openldap: 
```

And Enjoy ! 

---

@DENIS Guillaume
