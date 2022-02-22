After creating the Dockerfile, the new image is build using:

```sh
ishraque@ishraque-laptop:~$ sudo docker build . -f PART-01/1.7/Dockerfile -t web-server
```

The following output is seen:

```sh
Sending build context to Docker daemon  116.2kB
Step 1/2 : FROM devopsdockeruh/simple-web-service:alpine
 ---> fd312adc88e0
Step 2/2 : CMD server
 ---> Running in 220df11ca2a2
Removing intermediate container 220df11ca2a2
 ---> 4a222177976d
Successfully built 4a222177976d
Successfully tagged web-server:latest
```

Then the following command is used to start a container of the image:

```sh
ishraque@ishraque-laptop:~$ sudo docker run web-server
```

The following output is as expected:

```sh
[GIN-debug] [WARNING] Creating an Engine instance with the Logger and Recovery middleware already attached.

[GIN-debug] [WARNING] Running in "debug" mode. Switch to "release" mode in production.
 - using env:   export GIN_MODE=release
 - using code:  gin.SetMode(gin.ReleaseMode)

[GIN-debug] GET    /*path                    --> server.Start.func1 (3 handlers)
[GIN-debug] Listening and serving HTTP on :8080
```