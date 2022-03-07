## Heroku App Link https://dwd-heroku-app.herokuapp.com/presses/new
---

The docker image is pulled from DockerHub using:
```sh
ishraque@ishraque-laptop:~$ sudo docker pull devopsdockeruh/heroku-example
```

Heroku cli is installed  and login using:
```sh
ishraque@ishraque-laptop:~$ sudo snap install heroku --classic; heroku login; \
                            heroku container:login
```

After logging into Heroku, the downloaded image is retagged and pushed to Heroku:
```sh
ishraque@ishraque-laptop:~$ docker tag devopsdockeruh/heroku-example registry.heroku.com/dwd-heroku-app/web; \
                            docker push registry.heroku.com/dwd-heroku-app/web
```

The application is released into Heroku with:
```sh
ishraque@ishraque-laptop:~$ heroku container:release -a dwd-heroku-app web
```
