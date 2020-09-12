# MongoDB :

### Connect with Mongo Shell 

**Run your connection string in your command line**

#### aggregate command

> db.collectionsname.aggregate( [ { $sort : { date : -1 }  } ] ).pretty()

#### remove command

> db.collection_name.remove({"_id " : ObjectId("---------ID HERE----------")})

# start mongo shell with username password 
```sh
$ mongo -u <username> -p <password> --authenticationDatabase admin
```
# mongodump 

Backup database from mongo-atlas (get mongo_uri from mongo-atlas [clusters > connect > connect your application ])
```sh
$ mongodump --uri=<mongo_uri>
```
# mongorestore:

Restore data after dump in local mongodb


```sh
$ mongorestore --host 127.0.0.1:27017 --username <username> --password <password> --authenticationDatabase admin --db test --verbose dump/test/
```


