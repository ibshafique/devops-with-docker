To complete this, we need to update apt repository and install curl within the container.

This can be done with:

```sh
ishraque@ishraque-laptop:~$ sudo docker run -it --rm --name ex1.4 ubuntu sh -c 'apt update; apt install -y curl; \
echo "Input website:"; read website; echo "Searching.."; \
sleep 1; curl http://$website;'
```

After inputing helsinki.fi as input, the output shown is as following:

```sh
<!DOCTYPE HTML PUBLIC "-//IETF//DTD HTML 2.0//EN">
<html><head>
<title>301 Moved Permanently</title>
</head><body>
<h1>Moved Permanently</h1>
<p>The document has moved <a href="https://www.helsinki.fi/">here</a>.</p>
</body></html>
```