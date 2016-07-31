# hibernate-verisoning-object-example
Hibernate Versioning Example, Hibernate Versioning Of Objects


Once an object is saved in a database, we can modify that object any number of times , If we want to know how many no of times that an object is modified then we need to apply this versioning concept.
When ever we use versioning then hibernate inserts version number as zero, when ever object is saved for the first time in the database.Later hibernate increments that version no by one automatically when ever a modification is done on that particular object.

In order to use this versioning concept, we need the following two changes in our application
Add one property of type int in our pojo class
In hibernate mapping file, add an element called version soon after id element

No need to add column to datbase (Hibernate will automatically create new column if it is not there)
