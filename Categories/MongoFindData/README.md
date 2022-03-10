> With this function, you can pull the data you want from the database.

------------

### Syntax:
```javascript
    mongo_find_data(filter, object, variable_name)
```
|Parameters   | Description  |
| :------------ | :------------ |
| filter  | The find action returns the first document in the collection that matches this filter. If you do not specify a filter, the action matches all document in the collection.  |
| object  | If you want to synchronize the variable of which instance, write that instance. If you want to change the variable in the object where the code is run, use self.  |
|  variable_name | If you want to change which variable of the instance you entered, enter the name of that variable.  |

------------


### Returns:
`Struct`

*Example Return:*
`{ "document": { "_id": "619..", "name": "Enes", "score" : 0 } }`

------------

### Example:
##### Current Data:
 ![](https://i.hizliresim.com/puza8di.png)
```javascript
test = -1;
my_database_1.mongo_find_data({ "score" : 0 }, self, "test")
 ```
*When this code finds the first data with a score of 0 in the database, it will assign it to the "test" variable in its object.*

##### Getting the first data in the Database
```javascript
test = -1;
my_database_1.mongo_find_data(mongo_all, self, "test")
 ```
*If you type mongo all in the filter section it will return you the first value in the database*
