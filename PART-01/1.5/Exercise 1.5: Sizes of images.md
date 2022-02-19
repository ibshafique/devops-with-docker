The alpine version of the container can be pulled using:
```sh
ishraque@ishraque-laptop:~$ sudo docker pull devopsdockeruh/simple-web-service:alpine
```

The images can be listed and compared using the following:
```sh
ishraque@ishraque-laptop:~/Desktop/Project/devops-with-docker$ sudo docker image ls
REPOSITORY                          TAG       IMAGE ID       CREATED         SIZE
ubuntu                              latest    54c9d81cbb44   2 weeks ago     72.8MB
devopsdockeruh/simple-web-service   ubuntu    4e3362e907d5   11 months ago   83MB
devopsdockeruh/simple-web-service   alpine    fd312adc88e0   11 months ago   15.7MB
```

The container can be run and then entered using:
```sh
ishraque@ishraque-laptop:~$ sudo docker run -d --rm --name ex1.5 devopsdockeruh/simple-web-service:alpine
f175ebddb00ce5734ea3a8ea7d76fe9541fea3519c02864dbe918a4375149166
ishraque@ishraque-laptop:~$ sudo docker exec -it ex1.5 sh
```

The log can be viewed using and the output is:
```sh
ishraque@ishraque-laptop:~/Desktop/Project/devops-with-docker$ sudo docker exec -it ex1.5 sh
/usr/src/app # tail -f ./text.log 
2022-02-17 20:27:39 +0000 UTC
2022-02-17 20:27:41 +0000 UTC
Secret message is: 'You can find the source code here: https://github.com/docker-hy'
2022-02-17 20:27:43 +0000 UTC
2022-02-17 20:27:45 +0000 UTC
2022-02-17 20:27:47 +0000 UTC
2022-02-17 20:27:49 +0000 UTC
2022-02-17 20:27:51 +0000 UTC
Secret message is: 'You can find the source code here: https://github.com/docker-hy'
2022-02-17 20:27:53 +0000 UTC
2022-02-17 20:27:55 +0000 UTC
2022-02-17 20:27:57 +0000 UTC
2022-02-17 20:27:59 +0000 UTC
2022-02-17 20:28:01 +0000 UTC
```

