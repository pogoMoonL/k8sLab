# Docker 

## Command 

* docker ps -a



## docker-compose

```shell
$ docker-compose up
```

```yml
version: "3"
services:
  db:
    image: mysql/mysql-server:5.7
    restart: always
    environment:
      MYSQL_USER: test
      MYSQL_PASSWORD: test
      MYSQL_ROOT_PASSWORD: test
      MYSQL_DATABASE: testdb
    ports:
      - 3306:3306

```