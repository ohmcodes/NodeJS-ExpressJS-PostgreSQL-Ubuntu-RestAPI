# NodeJS-ExpressJS-PostgreSQL-Ubuntu-RestAPI
Rest API using NodeJS ExpressJS PostgreSQL Ubuntu


# Requirements
  - Ubuntu 20 LTS
  - NodeJS
  - ExpressJS
  - PostgreSQL
  
# Update and Upgrade
```
sudo apt update
sudp apt upgrade
```

# Creating Virtual Environment
Note Change <env_name> to your desired environment name
```
virtualenv -p python3 <env_name>
cd <env_name>

ACTIVATE ENVIRONMENT
source bin/activate
```

# Clone repo
Note Change repo name <desired_foldername>
```
git clone https://github.com/ohmcodes/NodeJS-ExpressJS-PostgreSQL-Ubuntu-RestAPI.git <dersired_foldername>
```

# Install NPM
```
sudo apt install npm
```

# Install ExpressJS and Node-Postgres
```
npm i express pg
```

# Test Repo
```
node index.js

VISIT:
localhost:3000

OUTPUT:
{"info":"Node.js, Express, and Postgres API"}
```

# Create Database
Visit Tutorial (https://github.com/ohmcodes/Install-Postgresql-in-Ubuntu-and-Config)
```
dbname: nodetutsdb
username: nodetutsuser
password: nodetuts@123
```

# Create Table
```
sudo -u postgres psql

\c nodetutsdb

CREATE TABLE users (
  ID SERIAL PRIMARY KEY,
  name VARCHAR(30),
  email VARCHAR(30)
);

INSERT INTO users (name, email)
  VALUES ('Jerry', 'jerry@example.com'), ('George', 'george@example.com');
  
SELECT * FROM users;

\q
```

# Endpoints
```
GET /users
GET /users/:id
POST /users
PUT /users/:id
DELETE /users/:id
```




