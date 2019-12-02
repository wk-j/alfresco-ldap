## Alfresco LDAP

```
docker-compose up open-ldap
```

## Add
```
ldapadd -x -D "cn=admin,dc=example,dc=org" \
    -w admin \
    -f resource/new-user.ldif \
    -H ldap://localhost
```