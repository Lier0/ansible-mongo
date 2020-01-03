# ansible-mongo

Create a mongo cluster, with : mongoc, mongod, mongos services.
Primarily designed for a three nodes cluster on Debian 8 (systemd).

## Vars
```
mongo_cluster_name: mongo_cluster                                                   
mongod_port: 27017                                                              
mongoc_port: 27018                                                              
mongos_port: 27019 
```

## Scalability
Auto-scalable by ansible hosts file edition.
```
[mongo:children]
database
```

Take care : currently, all nodes have all the roles.

## TODO
Role separation.
