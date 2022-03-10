> With this function, you can delete the data you want from the database.

------------

### Syntax:
```javascript
    mongo_delete_data(filter, object, variable_name)
```
|Parameters   | Description  |
| :------------ | :------------ |
| filter  | The delete action deletes the first document in the collection that matches this filter.  |
| object  | If you want to synchronize the variable of which instance, write that instance. If you want to change the variable in the object where the code is run, use self.  |
|  variable_name | If you want to change which variable of the instance you entered, enter the name of that variable.  |

------------


### Returns:
`Struct`

*Example Return:*
`{ "deletedCount": 1 }`

------------

### Example:
```javascript
test = -1;
my_database_1.mongo_delete_data( {"score" : 0}, self, "test")
 ```
*This code will delete the first data in the database with a score value of 0.*
