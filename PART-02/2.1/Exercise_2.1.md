The docker-compose file is brought up with:
```sh
ishraque@ishraque-laptop:~$ sudo docker-compose -f PART-02/2.1/docker-compose.yml up -d
```

The log seems to be appearing in the text.log file in the host machine.

The docker-compose file is brought down with:
```sh
ishraque@ishraque-laptop:~$ sudo docker-compose -f PART-02/2.1/docker-compose.yml down -v
```