# CRUD Starter API

Start a CRUD api quickly using Node, Express & Postgres.

Serves four routes from one page with a separate function for get, post, put and delete requests.

All code can be edited and replaced to fit the needs of the project being built.

## Install Postgres &amp; Create a Database

Change the database to MYSQL. Be sure to change the database and credentials in server.js

```
brew services start postgresql
createdb crud-starter-api
```

**Open pSequel and create a table for our database**

```
CREATE TABLE testtable1 (
 id serial PRIMARY KEY,
 first VARCHAR(100),
 last VARCHAR(100),
 email text UNIQUE NOT NULL,
 phone VARCHAR(100),
 location VARCHAR(100),
 hobby VARCHAR(100),
 added TIMESTAMP NOT NULL
);
```