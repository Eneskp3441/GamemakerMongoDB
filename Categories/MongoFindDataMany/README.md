> With this function, you can pull the data you want from the database.

------------

### Syntax:
```javascript
    mongo_find_data_many(filter,sort={}, limit=100, object, variable_name)
```
|Parameters   | Description  |
| :------------ | :------------ |
| filter  | The find action returns documents in the collection that match this filter. If you do not specify a filter, the action matches all document in the collection. If the filter matches more documents than the specified limit, the action only returns a subset of them.  |
|sort |Matched documents are returned in ascending or descending order of the fields specified in the expression. |
|limit | The maximum number of matched documents to include in the returned result set. Each request may return up to 50,000 documents.|
| object  | If you want to synchronize the variable of which instance, write that instance. If you want to change the variable in the object where the code is run, use self.  |
|  variable_name | If you want to change which variable of the instance you entered, enter the name of that variable.  |

------------


### Returns:
`Array [Struct, Struct ...]`

*Example Return:*
`{ "documents": [{ "_id": "6193504e1be4ab27791c8133", "name": "Eneskp3441", "score" : 15 }] }`

------------

### Example:
```javascript
test = -1;
my_database_1.mongo_find_data_many({ "name" : "Eneskp3441" }, {"score" : 1}, 10, self, "test")
 ```
*This code will return a maximum of 10 of all data with "name" EnesKp3441 in the database and sorted by score, assign it to the variable "test" in its object.*

##### Get all data in database
```javascript
test = -1;
my_database_1.mongo_find_data_many(mongo_all,,, self, "test")
 ```
*If you type mongo_all in the filter section, it will return you all the values ​​in the database.*
