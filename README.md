# PouchDB_on_CouchDB
A sample project for running PouchDB on a CouchDB Showcase

These files are supposed to go into a CouchDB .

Open '''app.js''' and replace "todo" in ´var db = new PouchDB("todo");´ with your database URL (like <user>.iriscouch.com/<dbname>)
´´´
// EDITING STARTS HERE (you dont need to edit anything above this line)

  var db = var db = new PouchDB("todo");
  
```

In Futon create a new database and create a new document with the ID "webpage" and add the following files as attachments
 * app.js
 * base.css
 * bg.png 
 * index.html
 
To make it all work, one must enable CORS in the config (hope I or pouchDB can fix this in the future)

´´´
[httpd]
enable_cors = true

[cors]
origins = *
```

This is basically 
[A simple Task-list application in CouchDB](http://www.speqmath.com/tutorials/couchdb_tasklist/index.html)
with PouchDB support