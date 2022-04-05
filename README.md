# postgres-docker-template

This repository provides a simple `docker-compose.yml` file template to run postgres using docker. 

## Usage

The only dependency is docker (versions 19.03.0+).

Set your postgres username `POSTGRES_USER` and password `POSTGRES_PASSWORD` as environment variables. This can be done
using a `.env` file or using shell variables:
```
$ export POSTGRES_USER=<YOUR USERNAME>
$ export POSTGRES_PASSWORD=<YOUR PASSWORD>
```
For more information read the official [documentation](https://docs.docker.com/compose/environment-variables/).
<br>

To start, go to the root repository containing the `docker-compose.yml` file and run:
```
docker-compose up --detached
```
This will start a postgres instance listening on port 5432.

To terminate, run:
```
docker-compose down
```

