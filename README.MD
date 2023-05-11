# Database containers
This repository contains YML files for different docker configurations. The idea behind this is to just have one container for each type of database and when developing multiple projects it will be easier to handle.

When getting ready to deploy an application their might be a need to include each of these files within the project to have it managed on your servers.

## Databases included

 - MariaDB
 - MySQL 5.7
 - Postgres
 - SQL CE **(SOON TM)**
 - Redis **(SOON TM)**
 - Mongo DB **(SOON TM)**
 - Memcache **(SOON TM)**

## Commands
If you run

    docker-compose up
This will read the configuration from the `.ENV` file. On windows the separator for the files to run is `;` but in other OS it is `:` so you might need to update that.

Another way of running multiple `YML` configuration files is by using the -f flag.

    docker-compose -f mariadb.yml -f postgres.yml up
This will have the same effect as modifying the `.ENV` file.