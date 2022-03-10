> With this function, you can update the data you want from the database.

------------

### Syntax:
```javascript
    mongo_update_data(filter, new_data, object, variable_name)
```
|Parameters   | Description  |
| :------------ | :------------ |
| filter  | The update action modifies the first document in the collection that matches this filter.  |
|new_data |that specifies how to modify the matched document. |
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
my_database_1.mongo_update_data({"name" : "Eneskp3441"}, {"score" : 1}, self, "test");
 ```
*This code will set the score value of the first data with "name" EnesKp3441 to 1 in the database and assign it to the "test" variable in its own object.*
