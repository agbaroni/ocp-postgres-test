```
oc new-project dbms

oc new-app 'postgresql:13-el7~https://github.com/agbaroni/ocp-postgres-test.git' --name ania -e POSTGRESQL_USER=admin -e POSTGRESQL_DATABASE=test -e POSTGRESQL_PASSWORD='Admin123!'

oc logs -f buildconfig/postgres

oc apply -f service.yaml
```
