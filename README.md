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

* Describe database , tables 
```
\d <name>

\dt <name>
```
* Exit
```
\q
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