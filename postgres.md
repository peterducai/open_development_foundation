

# DOCKER/PODMAN

```
podman run --name postgresql -e POSTGRES_USER=myusername -e POSTGRES_PASSWORD=mypassword -p 5432:5432 -v /data:/var/lib/postgresql/data -d postgres
podman run --name my-pgadmin -p 82:80 -e 'PGADMIN_DEFAULT_EMAIL=user@domain.local' -e 'PGADMIN_DEFAULT_PASSWORD=postgresmaster'-d dpage/pgadmin4
podman inspect postgresql -f “{{json .NetworkSettings.Networks }}”
```



# OCP

start with 

```
oc deployment ... -r 0
then set the needed env
oc set env deployment/<name> POSTGRESQL_USER=user POSTGRESQL_PASSWORD=pass POSTGRESQL_DATABASE=db
oc scale deployment/name --replicas=1
```