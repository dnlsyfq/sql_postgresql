# Python with Postgresql

**Library**
psycopg2

**PostgreSQL commands**
* List databases
```
\l
```

* List tables
```
\dt
```
* List users
```
\du
```

* Connect database from start 
```
psql -d <database>
```

* Describe database , tables 
```
\d <name>

\dt <name>
```
* Exit
```
\q
```

* Create new user 

```
CREATE ROLE <name>;
CREATE ROLE <name> WITH LOGIN;
CREATE ROLE userName WITH LOGIN PASSWORD `password`;
CREATE ROLE userName WITH CREATEDB LOGIN PASSWORD 'password';
CREATE ROLE userName WITH SUPERUSER;
CREATE ROLE userName WITH LOGIN PASSWORD 'password' SUPERUSER;
```

* Grant permission

```
GRANT SELECT ON <table> TO <username>;
GRANT SELECT, INSERT, UPDATE, DELETE ON <table> TO <name>;
GRANT ALL PRIVILEGES ON <table> TO <name>;
```
* find privileges of table

```
\dp <table>
```
* Revoke permission

```
REVOKE SELECT ON <table> FROM <name>;
REVOKE SELECT,INSERT,UPDATE, DELETE ON <table> FROM <user>;
REVOKE ALL PRIVILEGES ON <table> FROM <user>;

```

**SQL Commands**

* CREATE DATABASE 
```
CREATE DATABASE name;

CREATE DATABASE name OWNER username;
```

* DROP DATABASE
```
DROP DATABASE name;
```

* CREATE TABLE
```
CREATE TABLE tableName(
   column1 dataType1 PRIMARY KEY,
   column2 dataType2,
   column3 dataType3,
   ...
);
```

* DROP TABLE 
```
DROP TABLE <table>;
```