Create the container with:
```sh
ishraque@ishraque-laptop:~$ sudo docker run --rm -d --name ex1.3 devopsdockeruh/simple-web-service:ubuntu
```

Enter into the container with:
```sh
ishraque@ishraque-laptop:~$ sudo docker exec -it ex1.3 bash
```

The secret message is:

```sh
2022-02-17 19:24:02 +0000 UTC
2022-02-17 19:24:04 +0000 UTC
2022-02-17 19:24:06 +0000 UTC
2022-02-17 19:24:08 +0000 UTC
2022-02-17 19:24:10 +0000 UTC
Secret message is: 'You can find the source code here: https://github.com/docker-hy'
2022-02-17 19:24:12 +0000 UTC
2022-02-17 19:24:14 +0000 UTC
2022-02-17 19:24:16 +0000 UTC
2022-02-17 19:24:18 +0000 UTC
2022-02-17 19:24:20 +0000 UTC
Secret message is: 'You can find the source code here: https://github.com/docker-hy'
2022-02-17 19:24:22 +0000 UTC
2022-02-17 19:24:24 +0000 UTC
2022-02-17 19:24:26 +0000 UTC
2022-02-17 19:24:28 +0000 UTC
2022-02-17 19:24:30 +0000 UTC
Secret message is: 'You can find the source code here: https://github.com/docker-hy'
2022-02-17 19:24:32 +0000 UTC
2022-02-17 19:24:34 +0000 UTC
2022-02-17 19:24:36 +0000 UTC
2022-02-17 19:24:38 +0000 UTC
2022-02-17 19:24:40 +0000 UTC
Secret message is: 'You can find the source code here: https://github.com/docker-hy'
2022-02-17 19:24:42 +0000 UTC
2022-02-17 19:24:44 +0000 UTC
2022-02-17 19:24:46 +0000 UTC

```