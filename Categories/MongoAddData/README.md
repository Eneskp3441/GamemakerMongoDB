> With this function, you can add any data you want to your database.
 ```javascript
    my_database_1.mongo_add_data( {"name" : "Enes", "score" : 0 } )
```
------------

### Syntax:
 ```javascript
    mongo_add_data(data:struct)
```
------------


### Returns:
`None`

------------

### Example:
 ```javascript
    my_database_1		= new MongoInit("myName","myDatabase","myCluster")
    my_database_1.mongo_add_data( {"name" : "Enes", "score" : 0 } )
 ```
