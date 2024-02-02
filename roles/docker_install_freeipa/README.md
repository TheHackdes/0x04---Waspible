# FreeIPA

## Migrate from OpenLDAP to FreeIPA

```bash
kinit admin
ipa migrate-ds --bind-dn='cn=admin,dc=myorg,dc=intern' --with-compat ldap://openldap_app:389 \
  --user-container="ou=Users" \
  --group-container="ou=Groups" \
  --group-objectclass=posixGroup  \
  --continue \
  --group-overwrite-gid
```
