> With this function, you can update the data you want from the database.

------------

### Syntax:
```javascript
    mongo_update_data_many(filter, new_data, object, variable_name)
```
|Parameters   | Description  |
| :------------ | :------------ |
| filter  | The update action modifies all documents in the collection that match this filter.  |
|new_data |that specifies how to modify matched documents. |
| object  | If you want to synchronize the variable of which instance, write that instance. If you want to change the variable in the object where the code is run, use self.  |
|  variable_name | If you want to change which variable of the instance you entered, enter the name of that variable.  |

------------


### Returns:
`Struct`

*Example Return:*
`{ "matchedCount": 12, "modifiedCount": 12 }`

------------

### Example:
```javascript
test = -1;
my_database_1.mongo_update_data_many({"name" : "Eneskp3441"}, {"score" : 1}, self, "test");
 ```
*This code will set the point value of all data with "name" EnesKp3441 in the database to 1 and assign it to the variable "test" in its own object.*
