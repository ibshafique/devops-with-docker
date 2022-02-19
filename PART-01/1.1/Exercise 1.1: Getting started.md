To view the running containers:

```sh
ishraque@ishraque-laptop:~$ sudo docker ps -a
CONTAINER ID   IMAGE           COMMAND                  CREATED          STATUS                      PORTS                                                    NAMES
ebad15fd1d88   httpd           "httpd-foreground"       37 seconds ago   Up 35 seconds               80/tcp                                                   quizzical_montalcini
a3f37ca4ad4c   mysql           "docker-entrypoint.s…"   4 minutes ago    Exited (1) 4 minutes ago                                                             beautiful_turing
94c02f494bc4   nginx           "/docker-entrypoint.…"   7 minutes ago    Exited (0) 13 seconds ago                                                            goofy_bohr
```