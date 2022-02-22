After making the Dockerfile and the required curler.sh script, the image is build using:

```sh
ishraque@ishraque-laptop:~$ sudo docker build . -f PART-01/1.8/Dockerfile -t curler
```

```sh
Sending build context to Docker daemon  139.3kB
Step 1/5 : FROM ubuntu:20.04
 ---> 54c9d81cbb44
Step 2/5 : WORKDIR /usr/src/app
 ---> Using cache
 ---> 1586b886a62c
Step 3/5 : RUN apt update &&     apt install -y curl
 ---> Using cache
 ---> 7a3f05ebdb46
Step 4/5 : COPY PART-01/1.8/curler.sh .
 ---> Using cache
 ---> 2081809fa5ca
Step 5/5 : CMD ./curler.sh
 ---> Running in 493b0b9d3506
Removing intermediate container 493b0b9d3506
 ---> a0501c79ea60
Successfully built a0501c79ea60
Successfully tagged curler:latest
```

Then the container is run with:

```sh
ishraque@ishraque-laptop:~/Desktop/Project/devops-with-docker$ sudo docker run -it --rm curler 
```

The output is as expected:

```sh
Input website:
helsinki.fi
Searching..
<!DOCTYPE HTML PUBLIC "-//IETF//DTD HTML 2.0//EN">
<html><head>
<title>301 Moved Permanently</title>
</head><body>
<h1>Moved Permanently</h1>
<p>The document has moved <a href="https://www.helsinki.fi/">here</a>.</p>
</body></html>
```