# etl-db-env
ETL for historical data and development database

## Requirements:
* docker >= 17.12.0+
* docker-compose

## To Run:
`docker-compose up`

## Access to Jupyter Lab with PySpark: 
*  localhost:8888?token=`token`

For now you will have to grab the `token` value from the docker-compose up stdout

```
notebook_container |     To access the notebook, open this file in a browser:
notebook_container |         file:///home/jovyan/.local/share/jupyter/runtime/nbserver-7-open.html
notebook_container |     Or copy and paste one of these URLs:
notebook_container |         http://e643afef477d:8888/?token=54f3bf34463f369b2bc2b52be882930dfc9ead5f88da4cd1
notebook_container |      or http://127.0.0.1:8888/?token=54f3bf34463f369b2bc2b52be882930dfc9ead5f88da4cd1
```

## Access to postgres: 
* `localhost:5432`
* **Username:** postgres (as a default)
* **Password:** changeme (as a default)

To start a interactive terminal session:
`docker exec -it postgres_container psql -U postgres`

## Access to PgAdmin: 
* **URL:** `http://localhost:5050`
* **Username:** pgadmin4@pgadmin.org (as a default)
* **Password:** admin (as a default)

## Add a new server in PgAdmin:
* **Host name/address** `postgres`
* **Port** `5432`
* **Username** as `POSTGRES_USER`, by default: `postgres`
* **Password** as `POSTGRES_PASSWORD`, by default `changeme`



---
[See the Wiki for additional information](https://github.com/Philadelphia-Lawyers-for-Social-Equity/etl-db-env/wiki)