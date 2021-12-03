### To run container for each dependency (app, db):
```bash
docker-compose up -d build
```

### To run tests:
```bash
docker-compose exec web pytest .
```
- This runs the `pytest .` command in the container `web` composed in docker-compose.

### check db with psql
```bash
$ docker-compose exec db psql --username=hello_fastapi --dbname=hello_fastapi_dev
```
- list dbs: `\l`
- connect to db: `\c hello_fastapi_dev`
- show tables: `\dt`
- quit: `\q`