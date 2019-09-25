# etl-db-env
ETL for historical data and development database

**tmp workflow**

*build it* -- `$ docker build -t plse-rt-env`

*run it* -- `$ docker run --rm -P --name PLSE-RT-ENV plse-rt-env`

*connect to db --* `$ psql -h localhost -p 49153 -d docker -U docker --password`

...more to come
