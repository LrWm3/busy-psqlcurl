# busy-psqlcurl

A docker psqlcurl client which never exits, allowing `docker exec -it busy-psqlcurl` into the docker container to prototype psql and curl shell scripts in an alpine environment. Otherwise, they never seem to work properly.

## Features

:star: alpine:3.8

:star: sh

:star: curl

:star: psql + the pg_* crew

:star: unzip

## Usage

Simply run it in the background and then exec in as follows

```
docker run -d --name busy-psqlcurl williammarsman/busy-psqlcurl:0.1
docker exec -it busy-psqlcurl sh
```
