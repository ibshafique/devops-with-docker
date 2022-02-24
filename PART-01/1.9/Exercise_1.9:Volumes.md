An empty named ```text.log``` is created using:
```sh
sudo touch /PART-01/1.9/Exercise_1.9:Volumes.md/text.log
```

The following is used to run the container with a persistent volume attached to it:
```sh
sudo docker run --rm -it \
-v "$(pwd)/PART-01/1.9/text.log:/usr/src/app/text.log" \
devopsdockeruh/simple-web-service
```

The output saved in the file is:
```
2022-02-24 21:32:09 +0000 UTC
2022-02-24 21:32:11 +0000 UTC
2022-02-24 21:32:13 +0000 UTC
2022-02-24 21:32:15 +0000 UTC
2022-02-24 21:32:17 +0000 UTC
Secret message is: 'You can find the source code here: https://github.com/docker-hy'
2022-02-24 21:32:19 +0000 UTC
2022-02-24 21:32:21 +0000 UTC
2022-02-24 21:32:23 +0000 UTC
2022-02-24 21:32:25 +0000 UTC
2022-02-24 21:32:27 +0000 UTC
Secret message is: 'You can find the source code here: https://github.com/docker-hy'
2022-02-24 21:32:29 +0000 UTC
2022-02-24 21:32:31 +0000 UTC
2022-02-24 21:32:33 +0000 UTC
2022-02-24 21:32:35 +0000 UTC
2022-02-24 21:32:37 +0000 UTC
Secret message is: 'You can find the source code here: https://github.com/docker-hy'
2022-02-24 21:32:39 +0000 UTC
2022-02-24 21:32:41 +0000 UTC
2022-02-24 21:32:43 +0000 UTC
2022-02-24 21:32:45 +0000 UTC

```