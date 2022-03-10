> With this function, you can replace the data you want from the database.

------------

### Syntax:
```javascript
    mongo_replace_data(filter, replace_data, object, variable_name)
```
|Parameters   | Description  |
| :------------ | :------------ |
| filter  | The replace action overwrites the first document in the collection that matches this filter.  |
|replace_data |that specifies how to modify matched documents. |
| object  | If you want to synchronize the variable of which instance, write that instance. If you want to change the variable in the object where the code is run, use self.  |
|  variable_name | If you want to change which variable of the instance you entered, enter the name of that variable.  |

------------


### Returns:
`Struct`

*Example Return:*
`{ "matchedCount": 1, "modifiedCount": 1 }`

------------

### Example:
```javascript
test = -1;
my_database_1.mongo_replace_data( {"name" : "Eneskp3441"}, {"name" : "Eneskp3441", "score" : 0, "verify" : true}, self, "my_variable")
 ```
*This code will replace the "name" EnesKp3441 data in the database with the new data you specified.*
