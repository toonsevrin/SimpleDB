# SimpleDB
Simple java backed database to train database infra


##QUERY LANGUAGE

Uses SQLlike syntax, though this is an extremely simple Key-Value DB.

### Requests

#### Create

INSERT INTO `key` VALUE `value`

* Key:
* Value:

#### Read

SELECT `key`

* Key

Response also contains:

* Value

#### Update

UPDATE `value` WHERE key=`key`,value=`value`

* Key:
* Expected [OPTIONAL]: The expected value
* Upsert: Create record if non existent (default false)
* Updated: The new value


#### Delete
DELETE WHERE key=`key`,value=`value`
* Key:
* Expected [OPTIONAL]: The expected value

### Responses

* Matched: Records matched by query
* Updated: Records updated by query
* Created: Records created by query
* Deleted: Records deleted by query