The docker-compose file is brought up with:
```sh
ishraque@ishraque-laptop:~$ sudo docker-compose -f PART-02/2.1/docker-compose.yml up -d
```

The log seems to be appearing in the text.log file in the host machine.
```
...
Secret message is: 'You can find the source code here: https://github.com/docker-hy'
2022-03-08 01:53:46 +0000 UTC
2022-03-08 01:53:48 +0000 UTC
2022-03-08 01:53:50 +0000 UTC
2022-03-08 01:53:52 +0000 UTC
2022-03-08 01:53:54 +0000 UTC
Secret message is: 'You can find the source code here: https://github.com/docker-hy'
2022-03-08 01:53:56 +0000 UTC
2022-03-08 01:53:58 +0000 UTC
2022-03-08 01:54:00 +0000 UTC
2022-03-08 01:54:02 +0000 UTC
2022-03-08 01:54:04 +0000 UTC
Secret message is: 'You can find the source code here: https://github.com/docker-hy'
2022-03-08 01:54:06 +0000 UTC
2022-03-08 01:54:08 +0000 UTC
2022-03-08 01:54:10 +0000 UTC
2022-03-08 01:54:12 +0000 UTC
...
```


The docker-compose file is brought down with:
```sh
ishraque@ishraque-laptop:~$ sudo docker-compose -f PART-02/2.1/docker-compose.yml down -v
```
