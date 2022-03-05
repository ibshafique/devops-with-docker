## DockerHub Link: https://hub.docker.com/repository/docker/ibshafique/myfirstdockerrepo

---

Created a very simple container image that would display
```
Hello. This is my first Dockerhub Repository
```

The image is built using:
```sh
ishraque@ishraque-laptop:~$ sudo docker build . -f ./PART-01/1.15/Dockerfile -t ibshafique/myfirstdockerrepo:v1
```

The image is test-run with:
```sh
ishraque@ishraque-laptop:~$ sudo docker run --rm -it --name testcontainer ibshafique/myfirstdockerrepo:v1
Hello. This is my first Dockerhub Repository
```

The image is pushed to DockerHub with:
```sh
ishraque@ishraque-laptop:~$ sudo docker push ibshafique/myfirstdockerrepo:v1
```

---

The system can be cleaned with:
```sh
ishraque@ishraque-laptop:~$ sudo docker system prune -a
```

Now the image can be downloaded from DockerHub and run with:
```sh
ishraque@ishraque-laptop:~$ sudo docker run --rm -it --name testcontainer ibshafique/myfirstdockerrepo:v1
```

The following output is displayed:
```
Unable to find image 'ibshafique/myfirstdockerrepo:v1' locally
v1: Pulling from ibshafique/myfirstdockerrepo
7c3b88808835: Pull complete 
89ae85062117: Pull complete 
Digest: sha256:3e628f801901ced6186121ddd2bdb73954b213977633d2de970ccb3be978b1a9
Status: Downloaded newer image for ibshafique/myfirstdockerrepo:v1
Hello. This is my first Dockerhub Repository
```