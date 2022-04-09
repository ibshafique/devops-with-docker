The required directories ```example-frontend``` and ```example-backend``` are copied from PART02/2.6 to PART02/2.8.

The required changes are made to the ```docker-compose.yml``` file

The following command is used to run the containers:

```sh
ishraque@ishraque-laptop:~$ docker-compose -f ./PART-02/2.8/docker-compose.yml up -d
```

The following command is used to turn down the containers:

```sh
ishraque@ishraque-laptop:~$ docker-compose -f ./PART-02/2.8/docker-compose.yml down -v
```