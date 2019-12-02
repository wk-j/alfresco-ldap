## Alfresco LDAP

```
docker-compose up open-ldap
```

## Add
```
ldapadd -x -D "cn=admin,dc=example,dc=org" \
    -w admin \
    -f resource/billy.ldif \
    -H ldap://localhost

ldapadd -x -D "cn=admin,dc=example,dc=org" \
    -w admin \
    -f resource/joe.ldif \
    -H ldap://localhost

ldapadd -x -D "cn=admin,dc=example,dc=org" \
    -w admin \
    -f resource/beer.ldif \
    -H ldap://localhost
```

## Resource

- https://github.com/Acosix/alfresco-mt-support/wiki/Multi-Tenant-LDAP-Authentication-and-User-Registry